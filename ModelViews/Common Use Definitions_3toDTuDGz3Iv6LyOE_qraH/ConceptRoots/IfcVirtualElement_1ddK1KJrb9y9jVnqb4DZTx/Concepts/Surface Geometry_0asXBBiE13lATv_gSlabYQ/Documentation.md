The 3D geometric representation of _IfcVirtualElement_ is d efined using a surface geometry. The following constraints apply to the 3D surface representation:

<ul>
 
<li>'Surface3D': <em>IfcSurfaceOfLinearExtrusion</em>,
<em>IfcCurveBoundedPlane</em>, <em>IfcCurveBoundedSurface</em>,
<em>IfcRectangularTrimmedSurface</em></li>

 <li style="list-style-type: none;"><small>in case of an
<em>IfcSurfaceOfLinearExtrusion</em></small>

  <ul>
   
<li><small><u>Profile</u>:
<em>IfcArbitraryOpenProfileDef</em></small></li>
   
<li><small><u>Extrusion</u>: The extrusion direction shall be
vertically, i.e., along the positive Z Axis of the co-ordinate
system of the containing spatial structure element.</small></li>
  
</ul>

 </li>

 <li style="list-style-type: none;"><small>in case of an
<em>IfcCurveBoundedPlane</em>, <em>IfcCurveBoundedSurface</em>,
<em>IfcRectangularTrimmedSurface</em></small>
  
<ul>
   
<li><small><u>Extrusion</u>: The <em>BasisSurface</em> shall be a
surface that is upright, i.e. standing perpendicular to the xy
place of the co-ordinate system of the containing spatial
structure element.</small></li>

   </ul>

 </li>
 
<li>'GeometricSet': a list of 3D surfaces within the constraints
shown above.</li>

</ul>