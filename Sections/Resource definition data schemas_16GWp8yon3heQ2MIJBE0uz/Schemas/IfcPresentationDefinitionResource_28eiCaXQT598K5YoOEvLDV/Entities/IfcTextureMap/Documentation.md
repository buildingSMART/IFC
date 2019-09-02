**Definition
from IAI:** An _IfcTextureMap_ provides the mapping of the 2-dimensional texture coordinates to the surface onto which it is mapped. It is used for mapping the texture to vertex based geometry models, such as

* _IfcFacetedBrep_
* _IfcFacetedBrepWithVoids_
* _IfcFaceBasedSurfaceModel_
* _IfcShellBasedSurfaceModel_

The _IfcTextureMap_ provides a set of _TextureMaps_, each _IfcVertexBasedTextureMap_ holds a corresponding pair of lists:

1. a list of _TexturePoints_, currently of type _IfcCartesianPoint_, and
2. a list of&nbsp;_TexturesVertices_ of type _IfcTextureVertex_.


Each _IfcTextureVertex_ (given as S, T coordinates of
2
dimension) corresponds to the geometric coordinates of the _IfcCartesianPoint_
(given as X, Y, and
Z coordinates of 3 dimensions).
> <small><font color="#0000ff">HISTORY&nbsp;
New class
in IFC
Release 2x Edition 2. </font><br>
  <font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp; The <i>IfcTextureMap</i>
has changed by deleting the attribute <i>Texture</i>.
The attribute <i>TextureMaps</i>
has
been added.</font></small>

**Informal
propositions**:

1. All _TexturePoints_ in the list _TextureMaps_ of _IfcVertexBasedTextureMap_ shall be used by the vertex based geometry, to which this texture map is assigned to by using the _IfcAnnotationSurface.Item_ attribute.