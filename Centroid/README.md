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

![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3Dn_%7Bx%7D%5Ciint%5Climits_%7BA%7Dx%5E%7B2%7D%5C%20dA%3Dn_%7Bx%7D%5Ciint%5Climits_%7BA%7Dx%5E%7B2%7D%5Cfrac%7B%5Cpartial%20x%7D%7B%5Cpartial%20x%7D%5C%20dA%3D%5Cfrac%7B1%7D%7B3%7Dn_%7Bx%7D%5Ciint%5Climits_%7BA%7D%5Cfrac%7B%5Cpartial%20x%5E%7B3%7D%7D%7B%5Cpartial%20x%7D%5C%20dA)

 ![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3D%5Cfrac%7B1%7D%7B3%7Dn_%7Bx%7D%5Cint%5Climits_%7BL%7Dx%5E%7B3%7Dn_%7Bx%7D%5E%7Be%7D%5C%20dL)

 where, ![](https://latex.codecogs.com/gif.latex?n_%7Bx%7D%5E%7Be%7D)
  is the ![](https://latex.codecogs.com/gif.latex?x)-component of unit-normal to the edges of the triangle pointing outward of the triangle. For each of the edge of the triagle the normal is constant, therefore we can pull the normal outside of the integration,

  ![](https://latex.codecogs.com/gif.latex?I_%7Bx%7D%3D%5Cfrac%7B1%7D%7B3%7Dn_%7Bx%7D%5Csum_%7Bi%3D0%7D%5E%7B2%7Dn_%7Bxi%7D%5E%7Be%7D%5Cint%5Climits_%7BL_%7Bi%7D%7Dx%5E%7B3%7D%5C%20dL)

 The ![](https://latex.codecogs.com/gif.latex?x)-component of the centroid of a solid made-up of ![](https://latex.codecogs.com/gif.latex?N) triangles can be written as,

 ![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bx%7D%3D%5Cfrac%7B1%7D%7B6%7D%5Cfrac%7B1%7D%7BVolume%7D%5Csum_%7Bt%3D0%7D%5E%7BN-1%7Dn_%7Bx%7D%5Csum_%7Bi%3D0%7D%5E%7B2%7Dn_%7Bxi%7D%5E%7Be%7D%5Cint%5Climits_%7BL_%7Bi%7D%7Dx%5E%7B3%7D%5C%20dL)

 Similarly,

 ![](https://latex.codecogs.com/gif.latex?%5Cbar%7By%7D%3D%5Cfrac%7B1%7D%7B6%7D%5Cfrac%7B1%7D%7BVolume%7D%5Csum_%7Bt%3D0%7D%5E%7BN-1%7Dn_%7By%7D%5Csum_%7Bi%3D0%7D%5E%7B2%7Dn_%7Byi%7D%5E%7Be%7D%5Cint%5Climits_%7BL_%7Bi%7D%7Dy%5E%7B3%7D%5C%20dL)

 ![](https://latex.codecogs.com/gif.latex?%5Cbar%7Bz%7D%3D%5Cfrac%7B1%7D%7B6%7D%5Cfrac%7B1%7D%7BVolume%7D%5Csum_%7Bt%3D0%7D%5E%7BN-1%7Dn_%7Bz%7D%5Csum_%7Bi%3D0%7D%5E%7B2%7Dn_%7Bzi%7D%5E%7Be%7D%5Cint%5Climits_%7BL_%7Bi%7D%7Dz%5E%7B3%7D%5C%20dL)

 The line integrations can be carried out numerically using 3 or more quadrature points. To reduce the numerical error it is advisable to translate all the enclosing triangles of the solid close to the origin. This can be done by translation of the solid by \left(-x_{min},-y_{min},-z_{min}\right)
 . After calculation of the centroid, the centroid can be translated back by \left(x_{min},y_{min},z_{min}\right)
 .
