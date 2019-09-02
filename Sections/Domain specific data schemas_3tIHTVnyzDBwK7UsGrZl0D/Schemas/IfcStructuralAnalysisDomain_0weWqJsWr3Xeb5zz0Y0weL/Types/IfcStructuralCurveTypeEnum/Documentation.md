This type definition shall be used to distinguish between different types of structural 'curve' members, such as cables. The _IfcStructuralCurveTypeEnum_ type is referenced by the entity _IfcStructuralCurveMember_.

* **RIGID_JOINED_MEMBER**: A member with capacity to carry transverse and axial loads, i.e. a beam. Its actual joints may be rigid or pinned. Typically used in rigid frames.
* **PIN_JOINED_MEMBER**: A member with capacity to carry axial loads only, i.e. a link. Typically used in trusses.
* **CABLE**: A tension member which is able to carry transverse loads only under large deflection.
* **TENSION_MEMBER**: A member without compressional stiffness.
* **COMPRESSION_MEMBER**: A member without tensional stiffness.
* **USERDEFINED**: A specially defined member.
* **NOTDEFINED**: A member without further categorization.

> <font color="#0000FF" size="-1">HISTORY: New type in Release IFC2x

		  Edition 2. </font>
>