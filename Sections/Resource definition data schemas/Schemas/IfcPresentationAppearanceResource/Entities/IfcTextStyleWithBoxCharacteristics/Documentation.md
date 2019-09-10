**Definition
from IAI**: The text style with box characteristics allows the presentation of annotated text by specifying the characteristics of the character boxes of the text and the spacing between the character boxes.

> <small>
NOTE&nbsp; The <i>IfcTextStyleWithBoxCharacteristics</i>
is an entity that had been adopted from ISO 10303, Industrial
automation systems and integration&mdash;Product data
representation and exchange, Part 46: Integrated generic resources:
Visual presentation.</small>

The _IfcTextStyleWithBoxCharacteristics_ is mainly used to provide some compatibility with ISO10303. Its usage is restricted to monospace text fonts (having uniform character boxes) and simple vector based text fonts. For true text fonts however the use of _IfcTextStyleTextModel_ is required.

<table border="0" cellpadding="2" cellspacing="2" width="100%">
  <tbody>
    <tr>
      <td><img src="figures/ifctextstylewithboxcharacteristics_fig1.gif" alt="box angles" border="0" height="270" width="400"></td>
      <td><img alt="use of attributes" src="figures/ifctextstylewithboxcharacteristics_fig2.gif" height="264" width="556"></td>
    </tr>
    <tr>
      <td><small>Illustration
from ISO 10303-46, page 91</small></td>
      <td><small>Illustration
from IAI</small></td>
    </tr>
  </tbody>
</table>

> <small>
  <font color="#0000ff">NOTE&nbsp;
Corresponding
STEP name: text_style_with_box_characteristics. Please refer to ISO/IS
10303-46:1994, p. 123 for the final definition of the formal standard.
The four optional attributes <i>BoxHeight,
BoxWidth, BoxSlantAngle, BoxRotateAngle</i>
are included directly at the entity, and are not handled through the
box_characteristic_select selecting box_height, box_width,
box_slant_angle, box_rotate_angle, each being defined types.&nbsp;
The <i>CharacterSpacing</i>
attribute has been added from </font><font color="#0000ff" size="-1"><small>ISO/IS
10303-46:1994
entity </small></font><font color="#0000ff" size="-1"><small>text_style_with_spacing.</small></font></small>

> <small><font color="#0000ff">HISTORY&nbsp; New entity in
Release
IFC2x
Edition 2.</font></small>  
> <small><font color="#ff0000">IFC2x
Edition 3 CHANGE&nbsp; The
attribute item <i>CharacterSpacing</i>
has
been added.</font></small>
