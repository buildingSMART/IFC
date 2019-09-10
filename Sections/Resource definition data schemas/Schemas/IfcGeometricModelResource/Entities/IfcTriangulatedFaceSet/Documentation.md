The _IfcTriangulatedFaceSet_ is a tessellated face set with all faces being bound by triangles. The faces are constructed by implicit polylines defined by three Cartesian points. The coordinates of each point are provided by an index into an ordered list of Cartesian points provided by the two-dimensional list _CoordIndex_, where

* the first dimension of the two-dimensional list addresses the list of triangular faces; 
* the second dimension of the two-dimensional list provides exactly three indices into the _IfcCartesianPointList_ referenced by _Coordinates_ defined at the supertype _IfcTessellatedFaceSet_. Each index points to a Cartesian point being a vertex of the triangle. 

Optional the normals at each vertex, being perpendicular to the face for that triangle, can be provided by the two-dimensional list _NormalIndex_, where

* the first dimension of the two-dimensional list addresses the corresponding list of triangular faces; 
* the second dimension of the two-dimensional list provides exactly three indices into the _IfcDirectionList_ referenced by _Normals_ defined at the supertype _IfcTessellatedFaceSet_. Each index, corresponding to the index of vertices, points to a direction being the normal at this vertex of the triangle. 

Figure 1 shows the use of _IfcTriangulatedFaceSet_ without annotation. The diagram of the _IfcTriangulatedFaceSet_ represents the indices and the ordered list into which the indices point. The index starts with 1 (indexed as 1 to N), if the greatest index in _CoordIndex_ in N, then the _IfcCartesianPointList_ shall have N lists of 3:3 coordinates.

Figure 2 shows an _IfcTriangulatedFaceSet_ represented by  
_CoordIndex_: ((1,6,5), (1,2,6), (6,2,7), (7,2,3), (7,8,6), (6,8,5), (5,8,1), (1,8,4), (4,2,1), (2,4,3), (4,8,7), (7,3,4))  
_IfcCartesianPointList_: ((0.,0.,0.), (1.,0.,0.), (1.,1.,0.), (0.,1.,0.), (0.,0.,2.), (1.,0.,2.), (1.,1.,2.), (0.,1.,2.))

<table summary="">
      <tr>
        <td style="width: 450px">
          <img src="../../../../../../figures/ifctriangulatedfaceset_01.png" width="450" height="450" alt="IfcTriangulatedFaceSet_01">
        </td>
        <td>
          <blockquote>
            <img src="../../../../../../figures/ifctriangulatedfaceset_example-01.png" width="275" height="350" alt="IfcTriangulatedFaceSet_Example-01">
          </blockquote>
        </td>
      </tr>
      <tr>
        <td style="width: 450px">
          <p class="figure">Figure 1 &mdash; Triangulated face set
          </p>
        </td>
        <td>
          <p class="figure">Figure 2 &mdash; Triangulated face set geometry
          </p>
        </td>
      </tr>
    </table>

> NOTE&nbsp; The definition of _IfcTriangulatedFaceSet_ is based on the **indexedFaceSet**, and **indexedTriangleSet** defined in ISO/IEC 19775-1

> HISTORY&nbsp; New entity in IFC4.