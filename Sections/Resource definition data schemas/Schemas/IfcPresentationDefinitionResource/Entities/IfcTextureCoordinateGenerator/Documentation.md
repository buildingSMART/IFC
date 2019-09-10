**Definition
from IAI:** The _IfcTextureCoordinateGenerator_ describes a procedurally defined mapping function with input parameter to map 2D texture coordinates to 3D geometry vertices. The allowable _Mode_ values and input _Parameter_ need to be agreed upon in implementer agreements.

The following additional definitions from ISO/IEC FCD 19775:200x, the Extensible 3D ([X3D](http://www.web3d.org/x3d/specifications/x3d_specification.html){ target="_blank"}) specification, apply:

> TextureCoordinateGenerator supports the automatic generation of texture coodinates for geometric shapes. This node can be used to set the texture coordinates. The mode field describes the algorithm used to compute texture coordinates, the following modes are foreseen in X3D:  
> <font size="-1">SPHERE,
CAMERASPACENORMAL, CAMERASPACEPOSITION,
CAMERASPACEREFLECTIONVECTOR, SPHERE-LOCAL, COORD, COORD-EYE, NOISE,
NOISE-EYE, SPHERE-REFLECT, SPHERE-REFLECT-LOCAL</font>

> <font color="#0000ff" size="-1">HISTORY: New class
in IFC
Release 2x Edition 2.<br>
  </font><font color="#ff0000"><small>IFC2x
Edition 2 Addendum 2 CHANGE&nbsp; The <i>IfcTextureCoordinateGenerator</i>
has changed by deleting the attribute <i>Texture</i>.</small></font>