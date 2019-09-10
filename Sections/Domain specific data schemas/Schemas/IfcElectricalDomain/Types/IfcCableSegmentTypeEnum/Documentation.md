The _IfcCableSegmentTypeEnum_ defines the range of different types of cable segment that can be specified.

> HISTORY&nbsp; New type in IFC2x2. Core and busbar segment added in IFC4.

{ .spec-head}
Enumerated Item Definitions:

* **BUSBARSEGMENT**: Electrical conductor that makes a common connection between several electrical circuits. Properties of a busbar are the same as those of a cable segment and are captured by the cable segment property set.
* **CABLESEGMENT**: Cable with a specific purpose to lead electric current within a circuit or any other electric construction. Includes all types of electric cables, mainly several core segments or conductor segments wrapped together.
* **CONDUCTORSEGMENT**: A single linear element within a cable or an exposed wire (such as for grounding) with the specific purpose to lead electric current, data, or a telecommunications signal.
* **CORESEGMENT**: A self contained element of a cable that comprises one or more conductors and sheathing.The core of one lead is normally single wired or multiwired which are intertwined.
* **USERDEFINED**: User-defined type.
* **NOTDEFINED**: Undefined type.