**Definition
from IAI**: The _IfcRelAssociatesProfileProperties_ is an objectified relationship between non geometric profile properties (subtypes of _IfcProfileProperties_) and elements to which these properties apply, e.g. building elements and building element types as used within the structural engineering domain for steel, timber or concrete structures.

If the _ProfileSectionLocation_ attribute is given, it points to a shape aspect of the geometric or topological representation of the structural member. This allows the assignment of several profile properties (by many instances of _IfcRelAssociatesProfileProperties_) to accommodate varying profiles and members with different profile sections.

If the _ProfileOrientation_ attribute is given, it provides an orientation of the profile.

* For _IfcStructuralCurveMember_ it is a rotation about the longitudinal axis of the underlying curve, the x axis is determined by a line from the start vertex to the end vertex.&nbsp;
    * If the longitudinal axis is not parallel to the structural z axis of the structural coordinate system of the analysis model, i.e. the curve member is a beam (or non-vertical member), the _ProfileOrientation_ defaults to [0.,0.,1.] (if the z axis is not orthogonal to the x axis, an adjustment is made to maintain orthogonality, see function _IfcBuildAxes_ for an algorithm). The &beta; angle is then measured from the structural z axis to determine the location of the structural z axis of the profile.&nbsp;
    * If the longitudinal axis is&nbsp;parallel to the structural z axis of the structural coordinate system of the analysis model, i.e. the curve member is a column, the _ProfileOrientation_ defaults to [1.,0.,0.]. The &beta; angle is then measured from the structural x axis to determine the location of the structural z axis of the profile.

* If the _ProfileOrientation_ attribute is given as an _IfcDirection_, it would default to:
    * For 'beams' as [0., sin&beta;, cos&beta; ]
    * For 'columns' as [cos&beta;, -sin&beta;, 0.]


> <small> <font color="#0000ff">
HISTORY&nbsp; New entity
in Release IFC2x Edition 2.</font> </small>

> <small><font color="#ff0000">IFC2x
Edition 2
Addendum 1 CHANGE &nbsp;The entity <i>IfcRelAssociatesProfileProperties</i>
has been made a subtype of <i>IfcRelAssociates</i>. </font><br>
  <font color="#ff0000">IFC2x
Edition 3 CHANGE &nbsp;The entity <i>IfcRelAssociatesProfileProperties</i>
has changed by adding the attribute<i>ProfileOrientation</i>.</font></small>
