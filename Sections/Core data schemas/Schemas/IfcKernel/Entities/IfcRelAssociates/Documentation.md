The association relationship (_IfcRelAssociates_) refer to external sources of information (most notably a classification, library or document). There is no dependency implied by the association.

> <font size="-1">EXAMPLE: Further information may the given to
		the tank equipment (as subtype of <i>IfcProduct</i>) in terms of its
		classification and instruction documents, the source of the additional
		information is held external to the IFC project model. </font>

Association relationships can the established to objects (occurrences) or to types (both object types, _IfcTypeObject_, or partial types, _IfcPropertySetDefinition_).

> <font size="-1">EXAMPLE 1: The classification information for
		the tank equipment may be associated to the <i>IfcTypeProduct</i> (subtype of
		<i>IfcTypeObject</i>), defining the specific information for all occurrences of
		that tank in the project. Therefore the association of the (e.g.) Uniclass
		notation 'L6814' may be associated by a subtype of <i>IfcRelAssociates</i> to
		the type information.</font>

> <font size="-1">EXAMPLE 2: The classification information for a
		particular space within a building may the associated to the <i>IfcSpace</i>
		object (subtype of <i>IfcObject</i>), defining a particular occurrence of
		space. Therefore the association of the (e.g.) DIN notation 'HNF 1.5' may be
		associated by a subtype of <i>IfcRelAssociates</i> to the
		object.</font>

The association relationship establishs a uni-directional association. The subtypes of _IfcRelAssociates_ establishes the particular semantic meaning of the association relationship.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC
		Release 2x.</font>

> <font color="#FF0000" size="-1">NOTE: Users should not
		instantiate the entity <i>IfcRelAssociates</i> from IFC2x Edition2 onwards. It
		will be changed into an ABSTRACT supertype in future releases of
		IFC.</font>