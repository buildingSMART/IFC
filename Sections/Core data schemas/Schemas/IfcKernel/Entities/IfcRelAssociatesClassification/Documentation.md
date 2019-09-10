This objectified relationship (_IfcRelAssociatesClassification_) handles the assignment of a classification object (items of the select _IfcClassificationSelect_) to objects (subtypes of _IfcObject_).

The relationship is used to assign a classification notation or a classification reference to objects. A single notation can be applied to multiple objects. Depending on the type of the _RelatingClassification_, either a reference to a fully described classification system can be made, or just a reference using the classification code.

The inherited attribute _RelatedObjects_ define the objects to which the classification is applied. The attribute _RelatingClassification_ is the reference to a classification, applied to the object(s).

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC Release
		  2x.</font>
>