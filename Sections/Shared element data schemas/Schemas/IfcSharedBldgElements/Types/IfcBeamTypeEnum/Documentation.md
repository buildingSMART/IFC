This enumeration defines the different predefined types of beams that can further specify an _IfcBeam_ or _IfcBeamType_.

> HISTORY&nbsp; New enumeration type in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; The enumerators HOLLOWCORE and SPANDREL have been added.

{ .spec-head}
Enumerated Item Definitions:

* **BEAM**: A standard beam usually used horizontally. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "structural member for carrying load(s) between or beyond points of support, usually narrow in relation to its length and horizontal or nearly so" 
* **JOIST**: A beam used to support a floor or ceiling. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "one of a series of parallel beams, usually horizontal" 
* **HOLLOWCORE**: A wide often prestressed beam with a hollow-core profile that usually serves as a slab component.
* **LINTEL**: A beam or horizontal piece of material over an opening (e.g. door, window). 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "beam supporting load(s) over an opening" 
* **SPANDREL**: A tall beam placed on the facade of a building. One tall side is usually finished to provide the exterior of the building. Can be used to support joists or slab elements on its interior side. 
>> NOTE&nbsp; They are also referred to as "spandrel panels", which are parts of a facade and sometimes have supporting consoles for floor slabs integrated. 
* **T_BEAM**: A beam that forms part of a slab construction and acts together with the slab which its carries. Such beams are often of T-shape (therefore the English name), but may have other shapes as well, e.g. an L-Shape or an Inverted-T-Shape. 
>> NOTE&nbsp; In order to distinguish beams by shape, the assigned _IfcProfileDef_ subtypes provide the shape type and, if using a subtype of <small>IfcParameterizedProfileDef</small>, also the shape parameterization. 
* **USERDEFINED**: User-defined linear beam element.
* **NOTDEFINED**: Undefined linear beam element