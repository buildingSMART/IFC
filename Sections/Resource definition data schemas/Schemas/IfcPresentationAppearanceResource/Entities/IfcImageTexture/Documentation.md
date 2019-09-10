**Definition
from IAI:** An _IfcImageTexture_ provides a 2-dimensional distribution of the lighting parameters of a surface onto which it is mapped.

The following additional definitions from ISO/IEC FCD 19775:200x, the Extensible 3D ([X3D](http://www.web3d.org/x3d/specifications/x3d_specification.html)) specification, apply:

* The ImageTexture node defines a texture map by specifying an image file and general parameters for mapping to geometry. Texture maps are defined in a 2D coordinate system (s, t) that ranges from [0.0, 1.0] in both directions. The bottom edge of the image corresponds to the S-axis of the texture map, and left edge of the image corresponds to the T-axis of the texture map. The lower-left pixel of the image corresponds to s=0, t=0, and the top-right pixel of the image corresponds to s=1, t=1.
* The texture is read from the URL specified by the url [reference attribute]. When the url field contains no values ([]), texturing is disabled. Browsers shall support the JPEG and PNG image file formats. Support for the GIF format is also recommended (including transparency).

The following general recommendations for image file format support from ISO/IEC FCD 19775:200x, the Extensible 3D ([X3D](http://www.web3d.org/x3d/specifications/x3d_specification.html)) specification, also apply:

Texture nodes that require support for the PNG image format shall interpret the PNG pixel formats in the following way:

1.  Greyscale pixels without alpha or simple transparency are treated as intensity textures. 
2.  Greyscale pixels with alpha or simple transparency are treated as intensity plus alpha textures. 
3.  RGB pixels without alpha channel or simple transparency are treated as full RGB textures. 
4.  RGB pixels with alpha channel or simple transparency are treated as full RGB plus alpha textures. 

If the image specifies colours as indexed-colour (i.e., palettes or colourmaps), the following semantics should be used (note that `greyscale' refers to a palette entry with equal red, green, and blue values):

1.  If all the colours in the palette are greyscale and there is no transparency chunk, it is treated as an intensity texture. 
2.  If all the colours in the palette are greyscale and there is a transparency chunk, it is treated as an intensity plus opacity texture. 
3.  If any colour in the palette is not grey and there is no transparency chunk, it is treated as a full RGB texture. 
4.  If any colour in the palette is not grey and there is a transparency chunk, it is treated as a full RGB plus alpha texture. 

Texture nodes that require support for JPEG files shall interpret JPEG files as follows:

1.  Greyscale files (number of components equals 1) are treated as intensity textures. 
2.  YCbCr files are treated as full RGB textures. 
3.  No other JPEG file types are required. It is recommended that other JPEG files are treated as a full RGB textures.

Texture nodes that recommend support for GIF files shall follow the applicable semantics described above for the PNG format.

> <font color="#0000ff" size="-1"> NOTE Corresponding
X3D name: ImageTexture. Please refer to ISO/IEC FCD 19775:200x for the
definition of the formal standard. </font>
> 
> <font color="#0000ff" size="-1">HISTORY: New class
in Release IFC2x Edition 2.</font>
>
