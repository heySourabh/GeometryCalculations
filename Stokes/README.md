# Calculation of volume of a any solid

The Stokes method is probably the most useful method for calculation of volume for any solid shape.

The volume of a solid is defined as:

![](https://latex.codecogs.com/gif.latex?%5Ciiint%5Climits_%7BVol%7D%20dx%5C%20dx%5C%20dz)

We can re-write this as:

![](https://latex.codecogs.com/gif.latex?%5Ciiint%5Climits_%7BVol%7D%20%5Cfrac%7B%5Cpartial%20x%7D%7B%5Cpartial%20x%7D%5C%20dx%5C%20dx%5C%20dz)

Using the Stokes theorem (the divergence theorem) we can write:

![](https://latex.codecogs.com/gif.latex?%5Ciint%5Climits_%7BArea%7D%20x%7E%5C%2Cnx%5C%20dA)

where, ![](https://latex.codecogs.com/gif.latex?nx) is the x-component of the unit normal. This means that now we can calculate the volume by just carrying out surface integrals over enclosing volume surfaces.
We can easily break-down a enclosing surface into to a set of triangles. We must be cautious however that the **normal must be pointing outwards** and the points of the triangle must be in the **anti-clockwise direction**.

Since a triangle is a planar surface ![](https://latex.codecogs.com/gif.latex?nx) is a constant and can be moved out of the integral, which results in:

![](https://latex.codecogs.com/gif.latex?nx%5Ciint%5Climits_%7BArea%7D%20x%5C%2C%5C%20dA)

This basically is a formula for x coordinate of the centroid of the triangle, times nx times Area of triangle.

Let us consider a single triangle, with vertices *a*, *b* and *c*, the x-coordinate of the centroid can be easily calculated as:

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bx%7D%20%3D%20%28xa%20&plus;%20xb%20&plus;%20xc%29%20/%203)

Also, let us assume that the vertices are in an anti-clockwise direction. The two vectors formed by points *a-b* and *a-c* (vector ab and vector ac) can be used for calculation of the area of the triangle.

![](https://latex.codecogs.com/gif.latex?%5Cvec%7BA%7D%20%3D%20%5Cfrac%7B1%7D%7B2%7D%20%28%5Cvec%7Bab%7D%20%5Ctimes%20%5Cvec%7Bac%7D%29)

This will result in a vector, whose length is equal to area of the triangle and direction is such that it points outwards from the solid. Scaling the vector to unit length and taking its *x*-component will give us *nx*. Taking the magnitude will give area, *A*. Summation of all the contributions from sub-surfaces will give the volume as:

![](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D0%7D%5E%7Bn-1%7D%20nx_i%5C%2C%7CA_i%7C%5C%2C%20%5Cbar%7Bx%7D_i)

Which can be simplified to:

![](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D0%7D%5E%7Bn-1%7D%20%5Cvec%7BA%7D_%7Bix%7D%5C%2C%20%5Cbar%7Bx%7D_i)

where, ![](https://latex.codecogs.com/gif.latex?%5Cvec%7BA%7D_%7Bix%7D) is the x-component of the area vector, ![](https://latex.codecogs.com/gif.latex?%5Cvec%7BA%7D_i).

Therefore, the volume of a solid madeup of *n* enclosing surfaces can be written as:

![](https://latex.codecogs.com/gif.latex?%5Ctext%7BVolume%7D%20%3D%20%5Csum_%7Bi%3D0%7D%5E%7Bn-1%7D%20%5Cvec%7BA%7D_%7Bix%7D%5C%2C%20%5Cbar%7Bx%7D_i)

## Code
Below is a program written in Java, to calculate volume of any solid:
```java
/*
 * @author Sourabh Bhat (heySourabh@gmail.com)
 */

/**
 * Calculates the volume of a solid formed by a set of triangles.
 * The triangles must have points either all-clockwise or all-anti-clockwise,
 * looking from outside of the solid.
 *
 * @param triangles array of triangles
 * @return non-negative volume enclosed by the set of triangles
 */
public double volume(Triangle[] triangles) {
    double volume = 0.0;
    for (Triangle t : triangles) {
        volume += volumeUnder(t);
    }
    return Math.abs(volume);
}

private double volumeUnder(Triangle tri) {
    Point[] p = tri.points();
    double xbar = (p[0].x + p[1].x + p[2].x) / 3.0;
    Vector vab = new Vector(p[0], p[1]);
    Vector vac = new Vector(p[0], p[2]);

    double ax = vab.y * vac.z - vac.y * vab.z; // x-component of cross product

    return ax * xbar * 0.5;
}
```

A simple implementation of required classes is provided below. For more elaborate implementation look at the implementation in repository [CFDSolver](https://github.com/heySourabh/CFDSolver/blob/master/src/main/geom/Geometry.java).

```java
/**
 * @author Sourabh Bhat (heySourabh@gmail.com)
 */
public class Triangle {
    private final Point[] points;

    public Triangle(Point p0, Point p1, Point p2) {
        points = new Point[]{p0, p1, p2};
    }

    Point[] points() {
        return points;
    }
}
```
-----

```java
/**
 * @author Sourabh Bhat (heySourabh@gmail.com)
 */
public class Point {
    public final double x, y, z;

    public Point(double x, double y, double z) {
        this.x = x;
        this.y = y;
        this.z = z;
    }
}
```
-----

```java
/**
 * @author Sourabh Bhat (heySourabh@gmail.com)
 */
public class Vector {
    public final double x, y, z;

    public Vector(Point from, Point to) {
        this.x = to.x - from.x;
        this.y = to.y - from.y;
        this.z = to.z - from.z;
    }
}
```
