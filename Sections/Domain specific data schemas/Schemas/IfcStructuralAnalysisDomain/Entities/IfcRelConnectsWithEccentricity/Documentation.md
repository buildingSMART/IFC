The entity _IfcRelConnectsWithEccentricity_ adds the definition of eccentricity to the connection between a structural member and a structural connection (representing either a node or support).&nbsp;

> <font color="#0000ff"><small>HISTORY&nbsp; New
entity in Release IFC2x Edition 3.</small> </font>

**Use Definition**

**_Point Connection_**  
Instances of the entity _IfcRelConnectsWithEccentricity_shall be used to describe a connection with eccentricity between an instance of _IfcStructuralPointConnection_ and&nbsp;an instance of _IfcStructuralCurveMember_ or _IfcStructuralSurfaceMember_. The _RelatedStructuralConnection_ for point connections therefore has to be of type'_IfcStructuralPointConnection_'. The eccentricity is defined by a connection constraint being of type '_IfcConnectionPointGeometry_', or by its subtype '_IfcConnectionPointEccentricity_'. It refers to the _IfcVertexPoint_, used by the _IfcStructuralCurveMember_, or _IfcStructuralSurfaceMember_, that is used in this connection, and optionally to the _IfcVertexPoint_, used by the _IfcStructuralPointConnection_. In addition the eccentricity can be given by x, y, and z distance values.
