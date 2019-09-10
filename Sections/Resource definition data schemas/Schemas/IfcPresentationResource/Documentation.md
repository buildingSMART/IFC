The schema _IfcPresentationResource_ defines the resources used for geometric representations and presentations of styled items. The primary application of this resource is for defining the annotation occurrences of curve, text, filled area, symbol, and surfaces and particularly the definitions of fonts, colours and planar extents.

> <font color="#0000FF" size="-1">NOTE: The definitions of this
		resource of the IFC model have been taken from the International Standard
		10303: "Industrial automation systems and integration - Product data
		representation and exchange", Part 46 "Integrated generic resources: Visual
		presentation". The reference of the final international standard is ISO/IS
		10303-46:1994. The <i>IfcPresentationResource</i> refers to the clause 7,
		"Presentation resource schema" of the standard.</font>

The definitions taken from ISO/IS 10303-46:1994 have undergone a adaptation process, characterized by:

* adaptation of the IFC naming convention (inner majuscules and Ifc prefix)
* adaptation of the STEP entities, where multiple inheritance or non-exclusive inheritance (i.e. AND or ANDOR subtype constraints) are used
* selection of a subset of the IR, using subtype and select pruning
* dimensionality of geometric representation items defined at each item (not through the representation context)
* omission of the name attribute at the representation item

The semantic definitions of _IfcPresentationResource_ are defined following the adaptation of the **ISO/CD 10303-46:1992**, _Industrial
		Automation Systems and Integration: Product Data Representation and Exchange -
		Part 46: Integrated Generic Resources. Visual presentation_. The type, class, and function semantic definition sections follow the adapted wording of the working draft, which is clearly indicated and quoted at each reference.

The definitions of all parts of the _IfcPresentationResource_, that are taken from ISO10303-46 are explicitly excluded from the copyright of the International Alliance of Interoperability.

> <font color="#0000FF" size="-1">NOTE: For more information on
		the definitions as defined in the formal ISO standard please refer to: ISO/IS
		10303-46:1994, Industrial Automation Systems and Integration: Product Data
		Representation and Exchange - Part 46: Integrated generic resources: Visual
		presentation. The formal standard can be obtained through the local publishers
		of standards in each individual country.</font>

The following is within the scope of the current versions of the presentation resources:

* definition of presentation style attributes for realistic and symbolic visualizations of geometric and non-geometric displayable elements in the product information, including presentation styles for 
    * curve
    * text
    * filled area
    * symbol
    * surface 
* support of externally defined character fonts and symbols;
* support of pre defined character fonts and symbols;
* image control by a layer mechanism.
