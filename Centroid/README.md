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
, points outside from the solid.

Thus, we can evaluate the centroid by calculation of second moment of area over the enclosing surface of the solid. If we divide the enclosing surface into triangles, then for each of the triangle the normal remains constant and therefore can be moved out of the integral. Let us consider the ![](https://latex.codecogs.com/gif.latex?x)-coordinate of the centroid.
