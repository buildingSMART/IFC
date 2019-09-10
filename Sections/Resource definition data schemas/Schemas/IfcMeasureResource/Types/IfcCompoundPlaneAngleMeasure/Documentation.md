A compound measure of plane angle in degrees, minutes, seconds, and optionally millionth-seconds of arc.

> <font size="-1">NOTE: IfcCompoundPlaneAngleMeasure is used where angles need to be 
described to an accuracy as fine as one millionth of a degree and expressed as parts of an arc. It may be 
used for angular measurement by surveyors or for other angular measurements where precision is 
required. Another usage is exact or approximate global positioning against a geographic coordinate systems using longitude and latitude.
</font>

Type: LIST [3:4] OF INTEGER

The first integer measure is the number of degrees in the range {360; -360}The second integer measure is the number of minutes in the range {60; -60}The third integer measure is the number of seconds in the range {60; -60}The optional fourth integer measure is the number of millionth-seconds in the range {1 000 000; -1 000 000}

> <font size="-1" color="#0000FF">
  HISTORY New type in IFC Release 1.5.1.
</font>