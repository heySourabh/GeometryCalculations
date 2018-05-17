The centroid, ![](https://latex.codecogs.com/gif.latex?%5Cbar%7Br%7D), of a solid is defined as,

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Br%7D%20%3D%20%5Cfrac%7B1%7D%7BVolume%7D%5Ciiint%5Climits_%7BV%7Dr%5C%20dV)

where, ![](https://latex.codecogs.com/gif.latex?r) is a position vector. The centroid has a few very interesting properties such as:
1. For a homogeneous solid the _center of mass_ is located at the centroid
2. For any _linear function_, the average of the function inside the solid can be calculated by simply evaluating the function at the centroid point.

The calculation of the centroid of a solid can be done by using the divergence theorem to reduce the volume integral to area integral.

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Br%7D%3D%5Cfrac%7B1%7D%7BVolume%7D%5Ciiint%5Climits_%7BV%7D%5Cleft%28x%2Cy%2Cz%5Cright%29%5C%20dV%3D%5Cfrac%7B1%7D%7BVolume%7D%5Ciiint%5Climits_%7BV%7D%5Cleft%28x%5Cfrac%7B%5Cpartial%20x%7D%7B%5Cpartial%20x%7D%2Cy%5Cfrac%7B%5Cpartial%20y%7D%7B%5Cpartial%20y%7D%2Cz%5Cfrac%7B%5Cpartial%20z%7D%7B%5Cpartial%20z%7D%5Cright%29%5C%20dV)

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Br%7D%3D%5Cfrac%7B1%7D%7BVolume%7D%5Cfrac%7B1%7D%7B2%7D%5Ciiint%5Climits_%7BV%7D%5Cleft%28%5Cfrac%7B%5Cpartial%20x%5E%7B2%7D%7D%7B%5Cpartial%20x%7D%2C%5Cfrac%7B%5Cpartial%20y%5E%7B2%7D%7D%7B%5Cpartial%20y%7D%2C%5Cfrac%7B%5Cpartial%20z%5E%7B2%7D%7D%7B%5Cpartial%20z%7D%5Cright%29%5C%20dV)

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bx%7D%3D%5Cfrac%7B1%7D%7BVolume%7D%5Cfrac%7B1%7D%7B2%7D%5Ciint%5Climits_%7BA%7Dx%5E%7B2%7D%5C%20n_%7Bx%7D%5C%20dA)

![](https://latex.codecogs.com/gif.latex?%5Cbar%7By%7D%3D%5Cfrac%7B1%7D%7BVolume%7D%5Cfrac%7B1%7D%7B2%7D%5Ciint%5Climits_%7BA%7Dy%5E%7B2%7D%5C%20n_%7By%7D%5C%20dA)

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bz%7D%3D%5Cfrac%7B1%7D%7BVolume%7D%5Cfrac%7B1%7D%7B2%7D%5Ciint%5Climits_%7BA%7Dz%5E%7B2%7D%5C%20n_%7Bz%7D%5C%20dA)

where, ![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bx%7D)
, ![](https://latex.codecogs.com/gif.latex?%5Cbar%7By%7D)
and ![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bz%7D)
are the components of the centroid in ![](https://latex.codecogs.com/gif.latex?x)
, ![](https://latex.codecogs.com/gif.latex?y)
and ![](https://latex.codecogs.com/gif.latex?z)
directions respectively. The unit normal to the enclosing surface,
![](https://latex.codecogs.com/gif.latex?%5Chat%7Bn%7D%3D%5Cleft%28n_%7Bx%7D%2Cn_%7By%7D%2Cn_%7Bz%7D%5Cright%29)
, points outward of the solid.
Thus, we can evaluate the centroid by calculation of second moment of area over the enclosing surface of the solid.

If we divide the enclosing surface into triangles, then for each of the triangle the normal remains constant and therefore can be moved out of the integral. Let us consider the integration of ![](https://latex.codecogs.com/gif.latex?x)-coordinate for an individual triangle in space.

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3D%5Ciint%5Climits_%7BA%7Dx%5E%7B2%7D%5C%20n_%7Bx%7D%5C%20dA)

Since ![](https://latex.codecogs.com/gif.latex?n_%7Bx%7D)
is constant the integration becomes,

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3Dn_%7Bx%7D%5Ciint%5Climits_%7BA%7Dx%5E%7B2%7D%5C%20dA)

The area integration needs to be carried out in the plane of the triangular element. Let us consider an arbitrary triangle with vertex 0, 1, 2. Let us also consider a new 2-dimensional ![](https://latex.codecogs.com/gif.latex?u-v) co-ordinate system with origin at the vertex 0 of the triangle, the ![](https://latex.codecogs.com/gif.latex?u)-axis aligned to base of the triangle pointing towards vertex 1. The ![](https://latex.codecogs.com/gif.latex?v)-axis is perpendicular to the ![](https://latex.codecogs.com/gif.latex?u)-axis in the plane of the triangle. The integration therefore becomes,

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3Dn_%7Bx%7D%5Ciint%5Climits_%7BA%7Dx%5E%7B2%7D%5C%20du%5C%2Cdv)

The integration can be vastly simplified by using natural co-ordinate system, ![](https://latex.codecogs.com/gif.latex?%5Cxi-%5Ceta), such that the ![](https://latex.codecogs.com/gif.latex?%5Cxi)-axis is aligned to ![](https://latex.codecogs.com/gif.latex?u)-axis and scaled such that the vertex 0 is at ![](https://latex.codecogs.com/gif.latex?%5Cxi%3D0) and vertex 1 is at ![](https://latex.codecogs.com/gif.latex?%5Cxi%3D1). The ![](https://latex.codecogs.com/gif.latex?%5Ceta)-axis is aligned to triangle edge 0-2 and scaled such that the vertex 0 is at ![](https://latex.codecogs.com/gif.latex?%5Ceta%3D0) and vertex 2 is at ![](https://latex.codecogs.com/gif.latex?%5Ceta%3D1). The region of integration in the ![](https://latex.codecogs.com/gif.latex?%5Cxi-%5Ceta) co-ordinate system therefore simplifies to a right-angled triangle, which is easy to integrate. The integrand, ![](https://latex.codecogs.com/gif.latex?x%5E%7B2%7D%5C%20du%5C%2Cdv), needs to be transformed for the ![](https://latex.codecogs.com/gif.latex?%5Cxi-%5Ceta) co-ordinate system. The linear transformation for ![](https://latex.codecogs.com/gif.latex?x) can be obtained as,

![](https://latex.codecogs.com/gif.latex?x%3Dc_%7B0%7D&plus;c_%7B1%7D%5Cxi&plus;c_%7B2%7D%5Ceta)

Now, substituting the constraints on the co-ordinate system, at ![](https://latex.codecogs.com/gif.latex?%5Cxi%3D0%2C%5Ceta%3D0);  ![](https://latex.codecogs.com/gif.latex?x%3Dx_%7B0%7D), we get,

![](https://latex.codecogs.com/gif.latex?x_%7B0%7D%3Dc_%7B0%7D&plus;c_%7B1%7D%5Ctimes0&plus;c_%7B2%7D%5Ctimes0)

![](https://latex.codecogs.com/gif.latex?c_%7B0%7D%3Dx_%7B0%7D)

Substituting, at ![](https://latex.codecogs.com/gif.latex?%5Cxi%3D1%2C%5Ceta%3D0);  ![](https://latex.codecogs.com/gif.latex?x%3Dx_%7B1%7D), we get,

![](https://latex.codecogs.com/gif.latex?x_%7B1%7D%3Dx_%7B0%7D&plus;c_%7B1%7D%5Ctimes1&plus;c_%7B2%7D%5Ctimes0)

![](https://latex.codecogs.com/gif.latex?c_%7B1%7D%3Dx_%7B1%7D-x_%7B0%7D)

Substituting, at ![](https://latex.codecogs.com/gif.latex?%5Cxi%3D0%2C%5Ceta%3D1); ![](https://latex.codecogs.com/gif.latex?x%3Dx_%7B2%7D), we get,

![](https://latex.codecogs.com/gif.latex?x_%7B2%7D%3Dx_%7B0%7D&plus;c_%7B1%7D%5Ctimes0&plus;c_%7B2%7D%5Ctimes1)

![](https://latex.codecogs.com/gif.latex?c_%7B2%7D%3Dx_%7B2%7D-x_%7B0%7D)

Therefore in the new co-ordinate system,

![](https://latex.codecogs.com/gif.latex?x%3Dx_%7B0%7D&plus;%5Cleft%28x_%7B1%7D-x_%7B0%7D%5Cright%29%5Cxi&plus;%5Cleft%28x_%7B2%7D-x_%7B0%7D%5Cright%29%5Ceta)

similarly,

![](https://latex.codecogs.com/gif.latex?y%3Dy_%7B0%7D&plus;%5Cleft%28y_%7B1%7D-y_%7B0%7D%5Cright%29%5Cxi&plus;%5Cleft%28y_%7B2%7D-y_%7B0%7D%5Cright%29%5Ceta)

and,

![](https://latex.codecogs.com/gif.latex?z%3Dz_%7B0%7D&plus;%5Cleft%28z_%7B1%7D-z_%7B0%7D%5Cright%29%5Cxi&plus;%5Cleft%28z_%7B2%7D-z_%7B0%7D%5Cright%29%5Ceta)

The integration now becomes,

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3Dn_%7Bx%7D%5Ciintop_%7BA%7D%5Cleft%5Bx_%7B0%7D&plus;%5Cleft%28x_%7B1%7D-x_%7B0%7D%5Cright%29%5Cxi&plus;%5Cleft%28x_%7B2%7D-x_%7B0%7D%5Cright%29%5Ceta%5Cright%5D%5E%7B2%7D%5C%20du%5C%2Cdv)

Also elemental area,

![](https://latex.codecogs.com/gif.latex?du%5C%2Cdv%3D%5Cfrac%7B1%7D%7B%5Cleft%7C%5Cpartial%5Cleft%28%5Cxi%2C%5Ceta%5Cright%29/%5Cpartial%5Cleft%28u%2Cv%5Cright%29%5Cright%7C%7Dd%5Cxi%5C%2Cd%5Ceta)

where, ![](https://latex.codecogs.com/gif.latex?%5Cleft%7C%5Cpartial%5Cleft%28%5Cxi%2C%5Ceta%5Cright%29/%5Cpartial%5Cleft%28u%2Cv%5Cright%29%5Cright%7C) is the determinant of the Jacobian. In this linear transformation
it is just the ratio of area of the triangle in the ![](https://latex.codecogs.com/gif.latex?%5Cxi-%5Ceta) co-ordinate
system to area of triangle in ![](https://latex.codecogs.com/gif.latex?u-v) co-ordinate system. Since the area of the triangle in ![](https://latex.codecogs.com/gif.latex?%5Cxi-%5Ceta) co-ordinate system is 0.5, the scaling factor becomes,

![](https://latex.codecogs.com/gif.latex?A_%7BT%7D%3D%5Cfrac%7B1%7D%7B%5Cleft%7C%5Cpartial%5Cleft%28%5Cxi%2C%5Ceta%5Cright%29/%5Cpartial%5Cleft%28u%2Cv%5Cright%29%5Cright%7C%7D%3D%5Cleft%7C%5Coverrightarrow%7B0-1%7D%5Ctimes%5Coverrightarrow%7B0-2%7D%5Cright%7C)

which is the magnitude of the cross-product of the vectors made from
edges 0-1 and 0-2. Therefore ![](https://latex.codecogs.com/gif.latex?A_%7BT%7D) is twice the area of the triangle.
The integration therefore becomes,

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3DA_%7BT%7D%5C%2Cn_%7Bx%7D%5Ciint%5Climits_%7BA%7D%5Cleft%5Bx_%7B0%7D&plus;%5Cleft%28x_%7B1%7D-x_%7B0%7D%5Cright%29%5Cxi&plus;%5Cleft%28x_%7B2%7D-x_%7B0%7D%5Cright%29%5Ceta%5Cright%5D%5E%7B2%7D%5C%20d%5Cxi%5C%2Cd%5Ceta)

with limits of the integration,

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3DA_%7BT%7D%5C%2Cn_%7Bx%7D%5Cintop_%7B%5Ceta%3D0%7D%5E%7B%5Ceta%3D1%7D%5C%20%5Cintop_%7B%5Cxi%3D0%7D%5E%7B%5Cxi%3D1-%5Ceta%7D%5Cleft%5Bx_%7B0%7D&plus;%5Cleft%28x_%7B1%7D-x_%7B0%7D%5Cright%29%5Cxi&plus;%5Cleft%28x_%7B2%7D-x_%7B0%7D%5Cright%29%5Ceta%5Cright%5D%5E%7B2%7D%5C%20d%5Cxi%5C%20d%5Ceta)

Using Maxima symbolic manipulator we can simplify this as,

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3DA_%7BT%7D%5C%2Cn_%7Bx%7D%5Cleft%28%5Cfrac%7Bx_%7B0%7D%5E%7B2%7D&plus;x_%7B1%7D%5E%7B2%7D&plus;x_%7B2%7D%5E%7B2%7D&plus;x_%7B0%7Dx_%7B1%7D&plus;x_%7B0%7Dx_%7B2%7D&plus;x_%7B1%7Dx_%7B2%7D%7D%7B12%7D%5Cright%29)

Therefore the formula for centroid of a solid with ![](https://latex.codecogs.com/gif.latex?N) enclosing triangles becomes,

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bx%7D%3D%5Cfrac%7B1%7D%7BVolume%7D%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D0%7D%5E%7BN-1%7DA_%7BTi%7D%5C%2Cn_%7Bxi%7D%5Cleft%28%5Cfrac%7Bx_%7B0%7D%5E%7B2%7D&plus;x_%7B1%7D%5E%7B2%7D&plus;x_%7B2%7D%5E%7B2%7D&plus;x_%7B0%7Dx_%7B1%7D&plus;x_%7B0%7Dx_%7B2%7D&plus;x_%7B1%7Dx_%7B2%7D%7D%7B12%7D%5Cright%29_%7Bi%7D)

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bx%7D%3D%5Cfrac%7B1%7D%7B24%7D%5Cfrac%7B1%7D%7BVolume%7D%5Csum_%7Bi%3D0%7D%5E%7BN-1%7DA_%7BTi%7D%5C%2Cn_%7Bxi%7D%5Cleft%28x_%7B0%7D%5E%7B2%7D&plus;x_%7B1%7D%5E%7B2%7D&plus;x_%7B2%7D%5E%7B2%7D&plus;x_%7B0%7Dx_%7B1%7D&plus;x_%7B0%7Dx_%7B2%7D&plus;x_%7B1%7Dx_%7B2%7D%5Cright%29_%7Bi%7D)

Similarly,

![](https://latex.codecogs.com/gif.latex?%5Cbar%7By%7D%3D%5Cfrac%7B1%7D%7B24%7D%5Cfrac%7B1%7D%7BVolume%7D%5Csum_%7Bi%3D0%7D%5E%7BN-1%7DA_%7BTi%7D%5C%2Cn_%7Byi%7D%5Cleft%28y_%7B0%7D%5E%7B2%7D&plus;y_%7B1%7D%5E%7B2%7D&plus;y_%7B2%7D%5E%7B2%7D&plus;y_%7B0%7Dy_%7B1%7D&plus;y_%7B0%7Dy_%7B2%7D&plus;y_%7B1%7Dy_%7B2%7D%5Cright%29_%7Bi%7D)

and

![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bz%7D%3D%5Cfrac%7B1%7D%7B24%7D%5Cfrac%7B1%7D%7BVolume%7D%5Csum_%7Bi%3D0%7D%5E%7BN-1%7DA_%7BTi%7D%5C%2Cn_%7Bzi%7D%5Cleft%28z_%7B0%7D%5E%7B2%7D&plus;z_%7B1%7D%5E%7B2%7D&plus;z_%7B2%7D%5E%7B2%7D&plus;z_%7B0%7Dz_%7B1%7D&plus;z_%7B0%7Dz_%7B2%7D&plus;z_%7B1%7Dz_%7B2%7D%5Cright%29_%7Bi%7D)

It is advisable to translate the solid close to the origin for the
numerical calculations so that the numerical errors due to squaring
of large numbers is reduced. The actual centroid can be obtained by
translating back by the same amount.
