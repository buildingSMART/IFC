**Definition
from ISO/CD 10303-46:1992**: The text style is a presentation style for annotation text..

**Definition
from IAI**: The _IfcTextStyle_ provides the text style table for presentation information assigned to text literals. The style is defined by color, text font characteristics, and text box characteristics. The definitions are based upon:

* definitions from ISO/IS 10303-46:1994 for (old) vector based and monospace text.   
* definitions from [Cascading Style Sheets, level 1](http://www.w3.org/TR/REC-CSS1){ target="_blank"}, W3C Recommendation 17 Dec 1996, revised 11 Jan 1999, CSS1, for all true type text. The use of the CSS1 definitions is the preferred way to represent text styles.


An _IfcTextStyle_,
when representing (old) vector based and
monospace text, is instantiated with:  
* _TextCharacterAppearance_:: _IfcTextStyleForDefinedFont_ (with _BackgroundColour_ = NIL)
* _TextStyle_:: _IfcTextStyleWithBoxCharacteristics_
* _TextFontStyle_:: _IfcDraughtingPreDefinedTextFont_ or _IfcExternallyDefinedTextFont_


An _IfcTextStyle_,
when representing (new) true type text, based
on CSS1 definitions, is instantiated with:  
* _TextCharacterAppearance_:: _IfcTextStyleForDefinedFont_
* _TextStyle_:: _IfcTextStyleTextModel_
* _TextFontStyle_:: _IfcTextStyleFontModel_

An _IfcTextStyle_ can be assigned to _IfcTextLiteral_ via the _IfcPresentationStyleAssignment_ through an intermediate _IfcAnnotationTextOccurrence_.

> <small>
  <font color="#0000ff">
NOTE&nbsp; Corresponding
STEP name: text_style. Please refer to ISO/IS 10303-46:1994 for the
final definition of the formal standard. In order to avoid ANDOR
subtype relationships, the <i>IfcTextBlockStyleSelect</i>
has been introduced that allows the combination of a text style as
having box characteristic, and/or having spacing, or having none of
those additional properties.</font></small>

> <small><font color="#0000ff">NOTE&nbsp;
Corresponding CSS1 definitions are: Font properties (font-family,
font-style, font-variant, font-weight, font-size), Color and background
properties (color, background-color) and Text properties (word-spacing,
letter-spacing, text-decoration, text-transform,
text-align, text-indent, line-height).</font></small>

> <small><font color="#0000ff">HISTORY&nbsp; New entity in
Release IFC2x
Edition 2.</font></small>  
> <small><font color="#ff0000">IFC2x
Edition 3
CHANGE&nbsp; The <i>IfcTextStyle</i>
has been changed
by adding <i>TextFontStyle</i>
and different data types for <i>TextStyle</i>
and <i>IfcCharacterStyleSelect</i>.<br>
  </font></small>