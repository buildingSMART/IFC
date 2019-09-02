Any _IfcElement_ (so far no further constraints are defined at the level of its subtypes) may be represented as a single or multiple Boundary Representation models (which are restricted to be faceted Brep's with or without voids). The Brep representation allows for the representation of complex element shape.

&nbsp;

<table>
 
<tr>
  
<td><img src="../../../figures/ifcbuildingelement-brep-layout1.gif" alt="Brep representation" border="0" height="275" width="400"></td>

  <td><blockquote class="example">EXAMPLE&nbsp; As shown in Figure 1, the Brep representation is given by an
 <em>IfcShapeRepresentation</em>, which includes one or more 
items, all of type <em>IfcFacetedBrep</em>. In some cases it may be useful to also expose a simple 
representation as a bounding box representation of the same complex 
shape.</blockquote> </td>
 </tr>

 <tr>
  
<td>
<p class="figure">Figure 1 &mdash; Building element body boundary
representation</p>
</td>
  <td>&nbsp;</td>
 </tr>


</table>