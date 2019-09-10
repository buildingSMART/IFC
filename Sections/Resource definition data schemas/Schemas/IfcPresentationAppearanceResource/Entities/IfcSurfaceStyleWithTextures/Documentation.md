**Definition
from IAI**: The entity _IfcSurfaceStyleWithTextures_ allows for the assignment of image textures to surface styles. These image textures can be applied repeating across the surface or mapped with a particular scale upon the surface.

The entity _IfcSurfaceStyleWithTextures_ is part of the surface style table for presentation information assigned to surfaces for shading, rendering and lighting with textures. The mapping of the texture onto the surface or the solid is determined by the texture coordinates, each _IfcAnnotationSurfaceOccurrence_ has a _TextureCoordinates_ attribute, referencing the texture coordinates for the occurrence of the _IfcSurfaceStyleWithTextures_.

> <small><font color="#0000ff">HISTORY&nbsp; This is a
new entity in IFC Release 2x Edition 2.
  </font></small>  
> <font color="#ff0000"><small>IFC2x Edition 3 CHANGE&nbsp; The <i>IfcSurfaceStyleWithTextures</i>
has been changed by deleting the inverse attribute <i>HasTextureCoordinates</i>, use
the <i>IfcAnnotationSurfaceOccurrence.TextureCoordinates</i> to
provide texture coordinates for each occurrence.</small></font>