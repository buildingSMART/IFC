**Definition
from IAI**: An IfcAnnotationSurface&nbsp;is a surface or solid with texture coordinates assigned. It provides the capabilities to assign

* surface shading information,
* surface rendering information
* surface lighting information
* surface textures

to a surface, or all surfaces of a face based surface model, a shell based surface model, or a solid model. If the assigned _IfcSurfaceStyle_ defines textures by including an instance of _IfcSurfaceStyleWithTextures_, the attribute _TextureCoordinates_ determines the mapping of the texture to the surface(s) of the _Item_. In case of vertex based geometry, texture maps may be used to define the texture coordinates for each face.&nbsp;

The style information is linked by using the _IfcStyledItem_ to the _IfcAnnotationSurface_ instance.

> <font color="#0000ff"><small>NOTE&nbsp;
No direct
corresponding STEP
entity, the entity has been defined in analogy to the other annotation
occurrence entity.</small> </font>

> <small><font color="#0000ff">HISTORY&nbsp;
New entity in
Release IFC2x Edition 3.</font></small>
