**Definition
from IAI:** An _IfcVertexBasedTextureMap_ provides the mapping of the 2-dimensional texture coordinates (S, T) to the vertices of a single surface onto which it is mapped. For each vertex coordinates, provided by _IfcCartesianPoin_, a set of 2 (S, T) texture coordinates are given.

The _IfcVertexBasedTextureMap_ provides two corresponding lists:

1. a list of&nbsp;_TexturePoints_, given by min. of 3 _IfcCartesianPoint_'s.
2. a list of&nbsp;_TextureVertices_, given by min. of 3 _IfcTextureVertex_'s.


These corresponding
lists are:  
> <tt>TextureVertices</tt><tt> --
LIST
[3:?] --o <b>IfcTextureVertex</b>
&nbsp;-- LIST [2:2] --o <b>IfcParameterValue<br>
  </b></tt><tt>TexturePoints
&nbsp; -- LIST [3:?] --o <b>IfcCartesianPoint</b>
-- LIST [3:3] --o <b>IfcLengthMeasure</b><br>
  </tt><tt><b></b></tt>


Each texture vertex (given as S, T coordinates of 2
dimension) corresponds to the geometric coordinates (given as X, Y, and
Z coordinates of 3 dimensions) of the Cartesian point, All Cartesian
points within the list of shall lie within a plane.
> <small>NOTE The application needs to
ensure that
the number of vertex points are
identical with the number of texture vertex coordinates and that both
lists correlate.</small>

> <small><font color="#0000ff">HISTORY&nbsp;
New class
in IFC
Release 2x Edition 2. </font><br>
  <font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp; The <i>IfcVertexBasedTextureMap</i>
has changed by deleting the attribute <i>VertexBasedGeometries</i>.
The attribute <i>TexturePoints</i> has been added.</font></small>  
>

**Informal
propositions**:

1. The list of _TextureVertices_ shall correspond to the list of _TexturePoints_.
2. All Cartesian points of the list of _TexturePoints_shall lie in one plane
3. The references points shall be part of the vertex based geometry to which the annotation surface&nbsp;with textures is assigned.