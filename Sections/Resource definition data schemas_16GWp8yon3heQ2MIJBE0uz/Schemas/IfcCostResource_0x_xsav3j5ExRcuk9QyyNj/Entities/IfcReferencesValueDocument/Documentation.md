An _IfcReferencesValueDocument_ is a means of referencing many instances of _IfcAppliedValue_ to a single document where the document is a price list, quotation, list of environmental impact values or other source of information.

> <font color="#0000FF" size="-1">HISTORY: New class in IFC
		Release 2x. Name changed from IfcReferencesCostDocument in IFC
		2x2</font>

**Use Definitions**

The purpose of this class is to be able to identify a reference source from which applied values are obtained. Since many objects may be obtain such values from the same referenced document, use of a relationship class allows the document to be identified once only when information is exchanged or shared rather than many times.