This enumeration defines the flow direction at a distribution port.

For pipe-based ports, the direction is the physical flow direction.

For duct-based ports, the direction is the physical flow direction.

For cable-based ports carrying electric power (circuits containing hot, neutral, ground), the direction is from the origination of power (from a distribution board to protective devices to switches to fixtures). For cable-based ports carrying communication signals, the direction originates from where the signal is shaped, such as a sensor. For communicaton networks, the direction originates from the up-level network host, such as a router (having _SOURCE_ ports) hosting multiple computers (having _SINK_ ports).

> HISTORY&nbsp; New enumeration in IFC2.0.

{ .spec-head}
Enumerated Item Definitions:

* **SOURCE**: A flow source, where a substance flows out of the connection.
* **SINK**: A flow sink, where a substance flows into the connection.
* **SOURCEANDSINK**: Both a source and sink, where a substance flows both into and out of the connection simultaneously.
* **NOTDEFINED**: Undefined flow direction.
