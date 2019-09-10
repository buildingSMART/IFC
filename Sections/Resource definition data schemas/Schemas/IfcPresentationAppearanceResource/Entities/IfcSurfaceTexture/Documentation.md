**Definition
from IAI:** An _IfcSurfaceTexture_ provides a 2-dimensional image-based texture map. It can either be given by referencing an external image file through an URL reference (_IfcImageTexture_), or by explicitly including an array of pixels (_IfcPixelTexture_).

The following additional definitions from ISO/IEC FCD 19775:200x, the Extensible 3D ([X3D](http://www.web3d.org/x3d/specifications/x3d_specification.html)) specification, apply:

* **Texture**: An image used in a texture map to create visual appearance effects when applied to geometry nodes.
* **Texture map**: A texture plus the general parameters necessary for mapping the texture to geometry.

Texture maps are defined by 2D images that contain an array of colour values describing the texture. The texture map values are interpreted differently depending on the number of components in the texture map and the specifics of the image format. In general, texture maps may be described using one of the following forms:

1.  Intensity textures (one-component)
2.  Intensity plus alpha opacity textures (two-component) 
3. Full RGB textures (three-component) 
4. Full RGB plus alpha opacity textures (four-component) 

> <font size="-1"><u>NOTE</u>:
Most image formats specify an alpha opacity, not transparency (where
alpha = 1 - transparency).</font>

> <font color="#0000ff" size="-1">HISTORY: New class
in Release IFC 2x Edition 2.</font>
