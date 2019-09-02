The opening direction is determined by the local placement of _IfcDoor_ and the _OperationType_ of the _IfcDoorType_ as shown in Figure 1. The _IfcDoorTypeOperationEnum_ defines the general layout of the door type and its symbolic presentation. Depending on the enumerator, the appropriate instances of _IfcDoorLiningProperties_ and _IfcDoorPanelProperties_ are attached in the list of _HasPropertySets_. The _IfcDoorTypeOperationEnum_ mainly determines the hinge side (left hung, or right hung), the operation (swinging, sliding, folding, etc.) and the number of panels.

> NOTE&nbsp; There are different definitions in various countries on what a left opening or left hung or left swing door is (same for right). Therefore the IFC definition may derivate from the local standard and need to be mapped appropriately.

<table><tr><td>
<table border="1" cellpadding="2" cellspacing="2" style=" width:90%;">

<thead>

 <tr>
  
<td align="left" valign="top"><small><b>Opening
directions</b></small></td>
  
<td align="left" valign="top">
<small><b>Definitions</b></small></td>
 
 <td align="left" valign="top"><small><b>Reference to other
standards</b></small></td>
 
</tr>

</thead>

<tbody>

 <tr valign="top">
  
<td><img src="../../../figures/ifcdoor-fig01.gif" height="130" width="150" alt="fig 1"></td>

  <td align="left"><small>The door panel (for swinging doors) opens
always into the direction of the positive Y axis of the local
placement. The determination of whether the door opens to the left
or to the right is done at the level of the <em>IfcDoorType</em>. 
Here it is a left side opening door given 
by <em>IfcDoorType.OperationType</em> = 
SingleSwingLeft</small></td>
  
<td align="left"><small>refered to as LEFT HAND (LH) in US *<br>
<br>
refered to as DIN-R (right hung) in Germany</small></td>
 
</tr>

 <tr valign="top">
  
<td><img src="../../../figures/ifcdoor-fig02.gif" height="130" width="150" alt="fig 2"></td>

  <td align="left"><small>If the door should open to the other side,
then the local placement has to be changed. It is still a left side 
opening door, given by <em>IfcDoorType.OperationType</em> =
 SingleSwingLeft</small></td>
  
<td align="left"><small>refered to as RIGHT HAND REVERSE (RHR) in
US *<br>
<br>
refered to as DIN-R (right hung) in Germany</small></td>
 
</tr>
 
<tr valign="top">
  
<td><img src="../../../figures/ifcdoor-fig03.gif" height="130" width="150" alt="fig 3"></td>
  
<td align="left"><small>If the door panel (for swinging doors)
opens to the right, a separate door style needs to be used (here
<em>IfcDoorTypee.OperationType</em> = SingleSwingRight) and it always 
opens into the direction of the positive Y axis of the local
placement.</small></td>
  
<td align="left"><small>refered to as RIGHT HAND (RH) in US *<br>
<br>
refered to as DIN-L (left hung) in Germany</small></td>

 </tr>

 <tr valign="top">
  
<td><img src="../../../figures/ifcdoor-fig04.gif" height="130" width="150" alt="fig 4"></td>
  
<td align="left"><small>If the door panel (for swinging doors)
opens to the right, and into the opposite directions, the local
placement of the door need to change. The door style is given by
<em>IfcDoorType.OperationType</em> = SingleSwingRight.</small></td>
  
<td align="left"><small>refered to as LEFT HAND REVERSE (LHR) in US
*<br>
<br>
refered to as DIN-L (left hung) in Germany</small></td>

 </tr>

</tbody>

<tfoot>
 
<tr valign="top">

  <td align="right" colspan="3"><small>* it assumes that the
'inside/private/primary' space is above (top in the pictures) and
 the 'outside/public/secondary' space is below (bottom in the
pictures).</small></td>
 </tr>

</tfoot>

</table>

</td></tr><tr><td><p class="figure">Figure 1 &mdash; Door swing</p></td></tr></table>

> NOTE&nbsp; The _OverallWidth_ and _OverallHeight_ parameters are for informational purpose only.