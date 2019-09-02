This objectified relationship (_IfcRelAssignsToProcess_) handles the assignment of an object as an item the process operates on. Process is related to the product that it operate on (normally as input or output) through this relationship. Processes can operate on things other than products, and can operate in ways other than input and output.

> **Example**, it may be common to define processes during estimating or scheduling that describe design tasks (resulting in documents), procurement tasks (resulting in construction materials), planning tasks (resulting in processes), etc. Furthermore, the ways in which process can operate on something might include "installs", "finishes", "transports", "removes", etc. The ways are described as operation types.

The inherited attribute _RelatedObjects_ gives the references to the objects, which the process operates on. The _RelatingProcess_ is the process, that operates on the object. The operation types are captured in the inherited attribute _Name_.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release 1.5.
		  Has been renamed from IfcRelProcessOperatesOn in IFC Release 2x.
		  </font>
>