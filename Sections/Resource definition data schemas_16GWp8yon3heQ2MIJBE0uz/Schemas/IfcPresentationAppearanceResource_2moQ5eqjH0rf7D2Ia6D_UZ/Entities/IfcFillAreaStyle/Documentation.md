**Definition
from ISO/CD 10303-46:1992**: The style for filling visible curve segments, annotation fill areas or surfaces with tiles or hatches.

**Definition
from IAI**: An _IfcFillAreaStyle_ provides the style table for presentation information assigned to annotation fill areas or surfaces for hatching and tiling. <font color="#0000ff">The
<i>IfcFillAreaStyle </i>defines
hatches as model hatches, i.e. the distance between hatch lines, or the
curve patterns of hatch lines are given in model space dimensions (that
have to be scaled using the target plot scale). </font>The _IfcFillAreaStyle_ allows for the following combinations of defining the style of hatching and tiling:

* Solid fill for areas and surfaces by only assigning _IfcColour_ to the set of _FillStyles_. It then provides the background colour for the filled area or surface.

> 
>> <small>NOTE&nbsp;
Color information of surfaces for
rendering is assigned by using <i>IfcSurfaceStyle</i>,
not by using <i>IfcFillAreaStyle</i>.</small>


> 
* Vector based hatching for areas and surfaces based on a single row of hatch lines by assigning a single instance of _IfcFillAreaStyleHatching_ to the set of _FillStyles_.
    * If an instance of _IfcColour_ is assigned in addition to the set of _FillStyles_, it provides the background colour for the hatching.

* Vector based hatching for areas and surfaces based on two (potentially crossing) rows of hatch lines by assigning two instances of _IfcFillAreaStyleHatching_ to the set of _FillStyles._
    * If an instance of _IfcColour_ is assigned in addition to the set of _FillStyles_, it provides the background colour for the hatching.


> 
>> <small>NOTE&nbsp;
Assigning more then two instances of <i>IfcFillAreaStyleHatching
</i>to
define three or more rows
of hatch lines is not encouraged.</small>_>>_


> 
* Tiling for areas and surfaces by assigning a single instance of _IfcFillAreaStyleTiles_ to the set of _FillStyles_.
    * If an instance of _IfcColour_ is assigned in addition to the set of _FillStyles_, it provides the background colour for the tiling.


> 
>> <small><font color="#ff0000">IFC2x Edition&nbsp;3
NOTE&nbsp; The use of IfcFillAreaStyleTiles is discouraged., as its
definition might change is future releases.</font><br> </small>


> 
* Externally defined hatch style by assigning a single instance of _IfcExternallyDefinedHatchStyle_ to the set of _FillStyles_.
    * If an instance of _IfcColour_ is assigned in addition to the set of _FillStyles_, it provides the background colour for the hatching.


Measures given to a hatch or tile pattern are given in
global
drawing length units.   
> <small>NOTE&nbsp;
Global units are defined at the single <i>IfcProject</i>
instance, given by <i>UnitsInContext:IfcUnitAssignment</i>,
the same
units are used for the geometric representation items and for the style
definitions.</small>
> 


The measure values for hatch or tile pattern <font color="#0000ff">apply to the
model space </font>with a target plot scale provided for the correct appearance in the default plot scale. For different scale and projection dependent fill area styles a different instance of _IfcFillAreaStyle_ needs to be used by _IfcPresentationStyleAssignment_ for different _IfcGeometricRepresentationSubContext_ dependent representations.

> <small>NOTE&nbsp;
the target plot scale is given by <i>IfcGeometricRepresentationSubContext.TargetScale</i>.</small>  
>
> 


An _IfcFillAreaStyle_ can be
assigned to _IfcFillArea_
via the _IfcPresentationStyleAssignment_
through an intermediate _IfcStyledItem_ or subtype _IfcAnnotationFillAreaOccurrence_.
> <font color="#0000ff" size="-1">
NOTE&nbsp; Corresponding
STEP name:
fill_area_style. Please refer to ISO/IS 10303-46:1994 for the final
definition of the formal standard. </font>
> 
> <font size="-1"><font color="#0000ff">HISTORY&nbsp;
New entity in
Release IFC2x Edition 2.</font> </font>
>