**Definition
from IAI**: The text style select allows for the selection of styles to be assigned to an annotated text. The text style determines the text model that affect the visual presentation of characters, spaces, words, and paragraphs. There are two choices:

* _IfcTextStyleWithBoxCharacteristics_for definitions from ISO/IS 10303-46:1994 for (old) vector based and monospace text.   
* _IfcTextStyleTextModel_ for definitions from [Cascading Style Sheets, level 1](http://www.w3.org/TR/REC-CSS1){ target="_blank"}, W3C Recommendation 17 Dec 1996, revised 11 Jan 1999, CSS1, for all true type text. The use of the CSS1 definitions is the preferred way to represent text styles.

> <font color="#0000ff"><small>HISTORY&nbsp;
New type in Release IFC2x Edition 2.</small>
  </font>  
> <font color="#ff0000"><small>IFC2x Edition 3 CHANGE&nbsp;
The items within the <i>IfcTextStyleSelect</i>
have changed to <i>IfcTextStyleWithBoxCharacteristics</i>
and <i>IfcTextStyleTextModel</i>.<br>
  </small></font>