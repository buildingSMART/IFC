The _IfcControllerTypeEnum_ defines the range of different types of controller that can be specified.

> HISTORY&nbsp; New enumeration in IFC2.0.

{ .change-ifc2x4}
> IFC4 CHANGE&nbsp; PROPORTIONALINTEGRAL and PROPORTIONALINTEGRALDERIVATIVE values deleted (property set enumeration now used). MULTIPOSITION added.

{ .spec-head}
Enumerated Item Definitions:

* **FLOATING**: Output increases or decreases at a constant or accelerating rate.
* **MULTIPOSITION**: Output is discrete value, can be one of three or more values.
* **PROGRAMMABLE**: Output is programmable such as Discrete Digital Control (DDC).
* **PROPORTIONAL**: Output is proportional to the control error and optionally time integral and derivative.
* **TWOPOSITION**: Output can be either on or off
* **USERDEFINED**: User-defined type.
* **NOTDEFINED**: Undefined type.