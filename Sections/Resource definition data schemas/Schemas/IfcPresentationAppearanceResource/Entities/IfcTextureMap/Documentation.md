﻿An _IfcTextureMap_ provides the mapping of the 2-dimensional texture coordinates to the surface onto which it is mapped. It is used for mapping the texture to surfaces of vertex based geometry models, such as

*  _IfcFacetedBrep_ 
*  _IfcFacetedBrepWithVoids_ 
*  _IfcFaceBasedSurfaceModel_ 
*  _IfcShellBasedSurfaceModel_ 

The _IfcTextureMap_ has a list of _TextureVertex_, that corresponds to the points of the outer face bound of the vertex based geometry item. The corresponding pair of lists is:

1. the list of _Polygon_ of the _IfcFaceOuterBound_ of type _IfcCartesianPoint_, and 
2. the list of _Vertices_ of type _IfcTextureVertex_. 

Each _IfcTextureVertex_ (given as S, T coordinates of the 2-dimension texture coordinate system) corresponds to the geometric coordinates of the _IfcCartesianPoint_ (given as 3-dimension X, Y, and Z coordinates within the object coordinate system of the geometric item).

{ .extDef}
> NOTE&nbsp; Definition according to ISO/IEC 19775-1:  
> The TextureCoordinate node is a geometry property node that specifies a set of 2D texture coordinates used by vertex-based geometry nodes to map textures to vertices.

> NOTE&nbsp; In contrary to the X3D vertext based geometry, for example IndexedFaceSet and ElevationGrid, the vertext based geometry in IFC may include inner loops. The areas of inner loops have to be cut-out from the texture applied to the outer loop.

<table summary="texture map use">
      <tr>
        <td>
          <img src="../../../../../../figures/ifctexturemap_fig-1.png" width="620" height="600" alt="IfcTextureMap_fig-1.png 35,6 KB">
        </td>
				<td style=" vertical-align:bottom;"><span style=" font-size:x-small;">Figure 1 illustrates applying a texture map to a vertex
      based geometry.</span>
				</td>
      </tr>
      <tr>
        <td>
          <p class="figure">Figure 1 &mdash; Texture map</p>
        </td>
				<td>&nbsp;</td>
      </tr>
    </table>

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; The attribute Texture is deleted, and the attribute TextureMaps is added.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; The attribute TextureMap is replaced by _Vertices_, and the attribute _AppliedTo_ is added.

{ .spec-head}
Informal Propositions:

1. The _IfcFace_ referenced in _AppliedTo_ shall be used by the vertex based geometry, to which this texture map is assigned to by through the _IfcStyledItem_.
