This enumeration defines the different types of linear elements an _IfcMember_ or _IfcMemberType_ object can fulfill.

> HISTORY&nbsp; New enumeration type in IFC2x2.

{ .change-ifc2x2}
> IFC2x2 CHANGE&nbsp; The additional identifiers CHORD, PLATE, STUD are added.

{ .change-ifc2x3}
> IFC2x3 CHANGE&nbsp; The additional identifier MULLION are added.

{ .spec-head}
Enumerated Item Definitions:

* **BRACE**: A linear element (usually sloped) often used for bracing of a girder or truss. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "structural member, usually diagonal, which acts in compression or tension and stiffens a structure" 
* **CHORD**: Upper or lower longitudinal member of a truss, used horizontally or sloped.
* **COLLAR**: A linear element (usually used horizontally) within a roof structure to connect rafters and posts.
* **MEMBER**: A linear element within a girder or truss with no further meaning.
* **MULLION**: A linear element within a curtain wall system to connect two (or more) panels.
* **PLATE**: A&nbsp;linear continuous horizontal element in wall framing, such as a head piece or a sole plate. 
>> NOTE&nbsp; The value PLATE shall not be mixed up with planar elements, such as sheets and panels, that are handled as _IfcPlate_ and _IfcPlateType_. 
* **POST**: A linear member (usually used vertically) within a roof structure to support purlins. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "light vertical member providing support" 
* **PURLIN**: A linear element (usually used horizontally) within a roof structure to support rafters 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "beam parallel to the eaves that gives intermediate support to rafters or roofing" 
* **RAFTER**: A linear elements used to support roof slabs or roof covering, usually used with slope. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "inclined structural member, usually arranged in series, that supports roofing in a pitched roof" 
* **STRINGER**: A linear element used to support stair or ramp flights, usually used with slope.
* **STRUT**: A linear element often used within a girder or truss. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "structural member intended to resist axial force(s) acting in compression" 
* **STUD**: Vertical element in wall framing. 
>> NOTE&nbsp; Term according to ISO6707-1 vocabulary "one of a series of vertical members in a partition or vertical structural members in a load bearing wall" 
* **USERDEFINED**: User-defined linear element.
* **NOTDEFINED**: Undefined linear element
