This objectified relationship handles the concatenation of processes over time. The sequence is defined as relationship between two processes. The related object is the successor of the relating object, being the predecessor. A time lag is assigned to a sequence, and the sequence type defines the way in which the time lag applies to the sequence.

_IfcRelSequence_ is defined as an one-to-one relationship, therefore it assigns one predecessor to one successor. However, each _IfcProcess_ can have multiple predecessors and successors, as the sequence relationship is truly an N-to-M relationship.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  1.0.
		  </font>
>