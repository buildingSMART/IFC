**Definition
from IAI**: This is a collection of structural properties applicable to all linear structural members having a profile definition. For the structural profile properties a further material dependent specialization is given for taking into account specific profile properties applicable only in the context of a specific building material.

> <font size="-1">NOTE: The radii of gyration are
not given
explicitly but can be derived from moment of inertia and section area.
For asymmetric profile the values for alpha and for the moments of
inertia of the principle axes can be calculated from <i>MomentOfInertiaY</i>,
  <i>MomentOfInertiaZ</i>
and <i>MomentOfInertiaYZ</i>.</font>
> 


The center of gravity is measured from the origin of the geometric profile definition (see subtypes of _IfcProfileDef_). The CentreOfGravityInX defines the distance along the geometric x axis of the geometric profile definition, the CentreOfGravityInY defines the distance along the geometric y axis.

* For parameterized profiles: Center of gravity is measured from the center of the profile definition, which is the center of the bounding box of that profile geometry.    
* For arbitrary profiles: Center of gravity is measured from the 0.,0. local origin of the underlying 2D coordinate system of the explicit profile definition.


The shear center is measured from the gravity center and is given in
the structural coordinates, defined by:  
* origin = center of gravity
* y axis = negative x axis of the geometric coordinate system
* z axis = negative y axis of the geometric coordinate system

> <small><font color="#0000ff">HISTORY&nbsp;
New entity
in Release IFC2x Edition 2.
  </font><br>
  <font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp; The <i>IfcStructuralProfileProperties</i>
has changed by adding the two attributes <i>CentreOfGravityInX</i>
and <i>CentreOfGravityInY</i>.</font></small>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2" width="860">
  <tbody>
    <tr>
      <td valign="top" width="405"><img alt="fig 1" src="figures/ifcstructuralprofileproperties_fig1.gif" height="300" width="400"><br>
      <small>For paramteric
profile definitions (here <i>IfcRectangleProfileDef</i>)
the center of gravity is relative to the center of the bounding box
(geometric center) and in case of profiles symmetrical to both axes it
is identical with the center of the bounding box.</small><br>
      <br>
      <small>About
the used y- and z-directions:<br>
For the profile position a two-dimensional coordinate system is defined
(see <i>IfcAxis2Placement2D</i>
or black axes in figure). The definition of the profile properties
(like <i>MomentOfInertiaY</i>)
is given according to the axis convention within structural engineering
(red axes in figure). See the figure below.</small><br>
      </td>
      <td valign="top" width="455"><img alt="fig 2" src="figures/ifcstructuralprofileproperties_fig2.gif" height="375" width="450"><br>
      </td>
    </tr>
    <tr>
      <td valign="top" width="405"><small>Figure
1: Definition of geometric and
structural coordinate
system</small></td>
      <td valign="top"><small>Figure
2: Definition of center of gravity and shear
center
for arbitrary profile definitions.</small></td>
    </tr>
  </tbody>
</table>