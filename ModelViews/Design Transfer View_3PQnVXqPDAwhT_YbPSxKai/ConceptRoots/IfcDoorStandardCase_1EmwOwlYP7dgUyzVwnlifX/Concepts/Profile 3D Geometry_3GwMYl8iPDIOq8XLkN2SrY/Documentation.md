The door profile is represented by a three-dimensional closed curve within a particular shape representation. The profile is used to apply the parameter of the parametric door representation. The following attribute values for the _IfcShapeRepresentation_ holding this geometric representation shall be used:

* _RepresentationIdentifier_ : 'Profile'
* _RepresentationType_ : 'Curve3D' or 'GeometricCurveSet', in case of 'GeometricCurveSet' only a single closed curve shall be contained in the set of _IfcShapeRepresentation.Items_.

The following additional constraints apply to the 'Profile' representation type:

* **Curve**: being an _IfcPolyline_ defining a rectangle.
* **Position**: The curve shall lie in the xz plane of the object placement coordinate (the y coordinate values of the _IfcCartesianPoint_'s shall be 0.).

&nbsp;

<table summary="">
 
<tr valign="top">

  <td><img src="../../../figures/ifcdoorstandardcase-01.png" alt="standard door" border="0" width="500" height="500"></td>

  <td>
<blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates applying the door lining parameters to the
door profile shape representation. The profile defines the outer
boundary to which the door lining parameters relate as:</blockquote>
   <blockquote>
<ul>

    <li class="small"><em>IfcDoorLiningProperties.LiningDepth</em> starting at distance
defined by <em>LiningOffset</em> going into the positive y
direction.</li>

    <li class="small"><em>IfcDoorLiningProperties.LiningThickness</em> offset into the
inner side of the rectangle.</li>
    <li class="small"><em>IfcDoorLiningProperties.LiningOffset</em> distance along the
positive y direction to where the <em>LiningDepth</em> applies.</li>
    
<li class="small"><em>IfcDoorLiningProperties.ThresholdThickness</em> starting at
the bottom edge of the rectangle into the inner side of the
rectangle</li>

    <li class="small"><em>IfcDoorLiningProperties.ThresholdDepth</em> starting at
distance defined by <em>LiningOffset</em> going into the positive y
direction.</li>
  
    <li class="small"><em>IfcDoorLiningProperties.TransomOffset</em> starting at the 
bottom edge of the rectangle (along local x axis) into the inner
side of the rectangle, distance provided as percentage of overall
height. Distance to the centre line of the transom.</li>
   
</ul></blockquote>
  
</td>

 </tr>

 <tr valign="top">
  
<td>
<p class="figure">Figure 1 &mdash; Door profile</p>
</td>
  
<td>&nbsp;</td>

 </tr>

</table>