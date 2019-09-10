The schema _IfcPresentationDimensioningResource_ defines the resources used for geometric representations and presentations of presentation callouts used for dimensioning. The primary application of this resource is for presenting the annotation occurrences of linear, radius, diameter and angular dimensions.

> <font color="#0000FF" size="-1">NOTE: The definitions of this
		resource of the IFC model have been taken from the International Standard
		10303: "Industrial automation systems and integration - Product data
		representation and exchange", Part 202 "Application protocol: Associative
		draughting". The reference is ISO/IS 10303-202:1996.</font>

The _IfcPresentationDimensioningResource_ contains all those definitions from ISO/IS 10303-202:1996, which are not already defined within the Integrated Resources of the International Standard 10303, namely in part 42 "Integrated generic resources: Geometric and topological representations", and part 46 "Integrated generic resources: Visual presentation". It contains such definitions that are used in ISO/IS 10303-202:1996, but are originally defined in part 101 "Integrated application resources: Draughting".

The definitions taken from ISO/IS 10303-202:1996 have undergone a adaptation process, characterized by:

* adaptation of the IFC naming convention (inner majuscules and Ifc prefix)
* adaptation of the STEP entities, where multiple inheritance or non-exclusive inheritance (i.e. AND or ANDOR subtype constraints) are used
* selection of a subset of the IR, using subtype and select pruning
* dimensionality of geometric representation items defined at each item (not through the representation context)
* omission of the name attribute at the representation item

The definitions taken from ISO/IS 10303-202:1996 are explicitly excluded from the copyright of the International Alliance of Interoperability.

> <font color="#0000FF" size="-1">NOTE: For more information on
		the definitions as defined in the formal ISO standard please refer to: ISO/IS
		10303-202:1996, Industrial Automation Systems and Integration: Product Data
		Representation and Exchange - Part 202: Application protocol: Associative
		draughting. The formal standard can be obtained through the local publishers of
		standards in each individual country.</font>