﻿This enumeration distinguishes between different types of structural surface members, such as the typical mechanical function of walls, slabs and shells.

> HISTORY&nbsp; New enumeration in IFC2x2.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; Renamed from _IfcStructuralSurfaceTypeEnum_.

{ .spec-head}
Enumerated Item Definitions:

* **BENDING_ELEMENT**: A member with capacity to carry out-of-plane loads, i.e. a plate.
* **MEMBRANE_ELEMENT**: A member with capacity to carry in-plane loads, for example a shear wall.
* **SHELL**: A member with capacity to carry in-plane and out-of-plane loads, i.e. a combination of bending element and membrane element.
* **USERDEFINED**: A specially defined member.
* **NOTDEFINED**: A member without further categorization.