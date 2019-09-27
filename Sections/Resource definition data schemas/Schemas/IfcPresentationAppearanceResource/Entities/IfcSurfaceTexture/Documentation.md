﻿An _IfcSurfaceTexture_ provides a 2-dimensional image-based texture map. It can either be given by referencing an external image file through an URL reference (_IfcImageTexture_), including the image file as a blob (long binary) into the data set (_IfcBlobTexture_), or by explicitly including an array of pixels (_IfcPixelTexture_).

The following definitions from ISO/IEC 19775-1 X3D Architecture and base components ([X3D Specification](http://www.web3d.org/x3d/specifications/)) apply:

<ul>
<li><span style="font-size:smaller;color:blue">Texture: An image
used in a texture map to create visual appearance effects when
applied to geometry nodes.</span></li>
<li><span style="font-size:smaller;color:blue">Texture map: A
texture plus the general parameters necessary for mapping the
texture to geometry.</span></li>
</ul>
Texture are defined by 2D images that contain an array of colour values describing the texture. The texture values are interpreted differently depending on the number of components in the texture and the specifics of the image format. In general, texture may be described using one of the following forms:

1. Intensity textures (one-component)
2. Intensity plus alpha opacity textures (two-component)
3. Full RGB textures (three-component)
4. Full RGB plus alpha opacity textures (four-component)

> NOTE&nbsp; Image formats specify an alpha opacity, not transparency (where alpha = 1 - transparency).
> 


Figure 1 illustrates the texture coordinate system.

!["texture coordinates"](../../../../../../figures/ifcsurfacetexture_fig-1.png "Figure 1 &mdash; Surface texture coordinates")

The following definitions from ISO/IEC 19775-1 X3D Architecture and base components ([X3D Specification](http://www.web3d.org/x3d/specifications/)) on texture coordinates apply:

* <span style="font-size:smaller;color:blue">Texture maps are defined in a 2D coordinate system (s,&nbsp;t) that ranges from [0.0, 1.0] in both directions. The bottom edge of the image corresponds to the S-axis of the texture map, and left edge of the image corresponds to the T-axis of the texture map. The lower-left pixel of the image corresponds to s=0, t=0, and the top-right pixel of the image corresponds to s=1, t=1. Texture maps may be viewed as two dimensional colour functions that, given an <em>(s,&nbsp;t)</em> coordinate, return a colour value <em>colour(s,&nbsp;t)</em>.</span>

If multiple surface textures are included in the _IfcSurfaceStyleWithTextures_ applying them to a geometric item, a mode and optional parameters can be included that blending operations.

The _RepeatS_ and _RepeatT_ Boolean flags control whether the texture map is repeated outside the [0.0, 1.0] texture coordinate range, when applied to a geometric surface, or clamped to lie within the [0.0, 1.0] range. The _TextureTransform_ applies a 2D non-uniform transformation to the texture before it is applied to a geometric surface.

The following definitions from ISO/IEC 19775-1 X3D Architecture and base components ([X3D Specification](http://www.web3d.org/x3d/specifications/)) apply:

<ul>
<li><span style="font-size:smaller;color:blue">These parameters
support changes to the size, orientation, and position of textures
on shapes. Note that these operations appear reversed when viewed
on the surface of geometry. For example, a <em>scale</em> value of (2
2) will scale the texture coordinates and have the net effect of
shrinking the texture size by a factor of 2 (texture coordinates
are twice as large and thus cause the texture to repeat). A
translation of (0.5 0.0) translates the texture coordinates +.5
units along the S-axis and has the net effect of translating the
texture &minus;0.5 along the S-axis on the geometry's surface. A
rotation of &pi;/2 of the texture coordinates results in a
&minus;&pi;/2 rotation of the texture on the geometry.</span></li>
<li><span style="font-size:smaller;color:blue">The <em>center</em>
field specifies a translation offset in texture coordinate space
about which the <em>rotation</em> and <em>scale</em> fields are
applied. The <em>scale</em> field specifies a scaling factor in S and
T of the texture coordinates about the <em>center</em> point.
<em>scale</em> values shall be in the range (&minus;&infin;,&infin;).
The <em>rotation</em> field specifies a rotation in radians of the
texture coordinates about the <em>center</em> point after the scale
has been applied. A positive rotation value makes the texture
coordinates rotate counterclockwise about the centre, thereby
rotating the appearance of the texture itself clockwise. The
<em>translation</em> field specifies a translation of the texture
coordinates.</span><br>
<span style="font-size:smaller">The following conventions
apply:</span>
<ul>
<li style="list-style-type:none"><span style="font-size:smaller">center =
<em>TextureTransform.LocalOrigin</em>;<br>
rotation = <em>TextureTransform.Axis1</em><br>
scale S = <em>TextureTransform.Scale</em><br>
scale T = <em>TextureTransform.Scale2</em></span></li>
</ul>
</li>
</ul>
> NOTE&nbsp; The definitions of texturing within this standard have been developed in dependence on the texture component of X3D. See ISO/IEC 19775-1.2:2008 X3D Architecture and base components Edition 2, Part 1, 18 Texturing component for the definitions in the international standard.

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Attribute TextureType replaces by _Mode_, attributes _Parameter_ and _MapsTo_ aded, new inverse attribute _UsedInStyle_.
