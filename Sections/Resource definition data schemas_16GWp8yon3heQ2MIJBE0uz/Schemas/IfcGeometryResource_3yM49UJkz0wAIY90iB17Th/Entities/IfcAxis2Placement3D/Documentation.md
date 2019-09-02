The _IfcAxis2Placement3D_ provides location and orientations to place items in a three-dimensional space. The attribute _Axis_ defines the Z direction, _RefDirection_ the X direction. The Y direction is derived.

> NOTE&nbsp; The _RefDirection_ does not have to be orthogonal to _Axis_.

If the attribute values for _Axis_ and _RefDirection_ are not given, the placement defaults to P[1] (x-axis) as [1.,0.,0.], P[2] (y-axis) as [0.,1.,0.] and P[3] (z-axis) as [0.,0.,1.].

<table>
      <tr>
        <td>
          <img src="../../../figures/ifcaxis2placement3d-layout1.gif" alt="axis2 placement 2D" border="0" height="300" width="400">
        </td>
        <td style="vertical-align:bottom">
          <blockquote class="note">
            Figure 1 illustrates the definition of the
            <em>IfcAxis2Placement3D</em> within the three-dimensional
            coordinate system.
          </blockquote>
        </td>
      </tr>
      <tr>
        <td>
          <p class="figure">Figure 1 &mdash; Axis2 placement 3D</p>
        </td>
        <td>
          &nbsp;
        </td>
      </tr>
    </table>

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> The location and orientation in three dimensional space of three mutually perpendicular axes. An axis2_placement_3D is defined in terms of a point (inherited from placement supertype) and two (ideally orthogonal) axes. It can be used to locate and orientate a non axi-symmetric object in space and to define a placement coordinate system. The entity includes a point which forms the origin of the placement coordinate system. Two direction vectors are required to complete the definition of the placement coordinate system. The axis is the placement Z axis direction and the ref_direction is an approximation to the placement X axis direction.

> NOTE&nbsp; Entity adapted from **axis2_placement_3d** defined in ISO10303-42.

> HISTORY&nbsp; New entity in IFC1.5.