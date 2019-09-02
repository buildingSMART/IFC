**Definition from ISO/CD 10303-46:1992**: An annotation fill area is a set of curves that may be filled with hatching, colour or tiling. The annotation fill are is described by boundaries which consist of non-intersecting, non-self-intersecting closed curves. These curves form the boundary of planar areas to be filled according to the style for the annotation fill area.

> <small> </small><small>NOTE: A curve that is not surrounded by any
other curve is a border between an unfilled area on the outside and a
filled area on the inside. Another curve may surround an unfilled area
if it is surrounded by another curve whose inside is a filled area.</small>
> 


**Illustration from ISO 10303-46**

![annotation fill area](figures/IfcAnnotationFillArea.gif)
> <font color="#0000ff"><small>NOTE&nbsp;
Corresponding STEP name: annotation_fill_area. Please refer to ISO/IS
10303-46:1994 for the final definition of the formal
standard.&nbsp;</small> </font>

&nbsp;The _IfcAnnotationFillArea_ defines an area by a definite _OuterBoundary_, that might include _InnerBoundaries_. The areas defined by the _InnerBoundaries_ are excluded from applying the fill area style.

Informal Proposition:

1. Any curve that describes an inner boundary shall not intersect with, nor include, another curve defining an inner boundary.
2. The curve defining the outer boundary shall not intersect with any curve defining an inner boundary, nor shall it be surrounded by a curve defining an inner boundary.

> <small><font color="#0000ff">HISTORY
New entity in Release IFC2x 2nd Edition.</font><br>
  <font color="#ff0000">IFC2x Edition 3 CHANGE
&nbsp;The two attributes <i>OuterBoundary</i> and <i>InnerBoundaries</i>
are added and replace the previous single boundary.</font></small>