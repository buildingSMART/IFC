The mapped item, _IfcMappedItem_, should be used if appropriate as it allows for reusing the geometry definition of a type at all occurrences of the same type.

A single instance of a subtype of _IfcElementComponent_ can stand for several actual element components at once. In this case, the _IfcShapeRepresentation_ contains as many mapped items as there are element components combined within this occurrence object.

&nbsp;

<table>

 <tr>
  <td><img src="../../../figures/ifcelementcomponent_multiple.png"></td>
  <td><blockquote class="example">EXAMPLE&nbsp; Figure 1 illustrates multiple components modeled as a single occurrence object (here: <em>IfcFastener</em>)</blockquote></td>
 </tr>
 
<tr>
  <td><p class="figure">Figure 1 &mdash; Element component mapped representation</p></td>
  <td><p>&nbsp;</p></td>
 </tr>

</table>

Representation identifier and type are the same as in single mapped representation. The number of mapped items in the representation corresponds with the count of element components in the _IfcElementQuantity_.