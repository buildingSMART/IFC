An _IfcDocumentReference_ is a reference to the location of a document. The reference is given by a system interpretable _Location_ attribute (e.g., an URL string) or by a human readable location, where the document can be found, and an optional inherited internal reference _ItemReference_, which refers to a system interpretable position within the document. The optional inherited _Name_ attribute is meant to have meaning for human readers. Optional document metadata can also be captured through reference to _IfcDocumentInformation_.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		Release 2.0. Modified in IFC 2x.</font>

### Use Definitions
Provides a lightweight capability that enables a document to be identified solely by reference to a name by which it is commonly known. The reference can also be used to point to document information for more detail as required.

For example, the IAI mission statement in a document "Introduction to IAI" can be referenced by _IfcDocumentReference.Location_ = 'http://iai-international.org/intro.html', and IfcDocumentReference = 'Mission statement'. Additionally: _IfcDocumentReference.ReferenceToDocument[1].Name_ = 'Introduction to IAI', and _IfcDocumentReference.ReferenceToDocument[1].Description_ = 'Basic document to introduce the aims of IAI'.
