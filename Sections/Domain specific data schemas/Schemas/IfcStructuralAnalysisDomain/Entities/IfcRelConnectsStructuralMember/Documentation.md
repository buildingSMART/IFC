The entity _IfcRelConnectsStructuralMember_ defines all needed properties describing the connection between structural members and structural connections (nodes or supports).

> <font size="-1">NOTE: The specification of frequently used connection
		  properties is done by using through the <i>AppliedCondition</i> attribute.
		  Rarely needed connection properties, such as slippage or failure, should be
		  specified by using the attribute <i>AdditionalConditions</i>.</font>
> 


> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
> 


**Use Definition**

_Point Connection_  
Instances of the entity _IfcRelConnectsStructuralMember_ shall be used to describe a connection between an instance of _IfcStructuralPointConnection_ and either an instance of _IfcStructuralCurveMember_ or _IfcStructuralSurfaceMember_. The _RelatedStructuralConnection_ for point connections has to be of type = 'IfcStructuralPointConnection'.

_Curve Connection_  
Instances of the entity _IfcRelConnectsStructuralMember_ shall be used to describe a connection between an instance of _IfcStructuralCurveConnection_ and an instance of either _IfcStructuralCurveMember_ or _IfcStructuralSurfaceMember_. The _RelatedStructuralConnection_ for curve connections has to be of type = 'IfcStructuralCurveConnection'.

_Surface Connection_  
Instances of the entity _IfcRelConnectsStructuralMember_ shall be used to describe a connection between an instance of _IfcStructuralSurfaceConnection_ and an instance of _IfcStructuralSurfaceMember_ (or an instance of a volumetric member, if defined in future extensions). The _RelatedStructuralConnection_ for curve connections has to be of type = 'IfcStructuralSurfaceConnection'.

_Coordinate System for Applied Conditions_  
All values defined by _AppliedCondition_ or _AdditionalConditions_ are given within the coordinate system provided by _ConditionCoordinateSystem_, which is defined in relation to the local coordinate system of the structural member. If the _ConditionCoordinateSystem_ is not defined, the local placement of the structural member is used instead.

_Supported Length_  
Optionally a supported length can be given, which gives the length (or width) of the physical connection along a curve connection.

!["supported length"](../../../../../../figures/ifcrelconnectsstructuralmember-fig1.gif "<font size="-1">Illustration of the appropriate definition of
				support lengths.</font>")
