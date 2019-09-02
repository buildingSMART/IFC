The abstract entity _IfcStructuralActivity_ combines the definition of actions (such as forces, displacement, etc) and reactions (supports and deformations) which are specified by using the basic load definitions from the_IfcStructuralLoadResource_. It also uses the inherited capabilities for the definition of a location and a local coordinate system.

The differentiation between actions and reactions is realized by instantiating objects either from subclasses of _IfcStructuralAction_ or _IfcStructuralReaction_ respectively. They inherit commonly needed attributes from the abstract superclass _IfcStructuralActivity_. Possible dependencies between actions and reactions must be explicitly captured.

The use of the location and local coordinate system, given by _ObjectPlacement_, is optional as it is not always needed or useful.

> <font size="-1">NOTE: Not needed if the 'activity' acts on the whole
		  element to which it is "connected" through an instance of
		  <i>IfcRelConnectsStructuralActivity</i> and additionally, there is no
		  eccentricity. It is not useful if the 'activity' acts on a building element
		  because at this stage no geometrical abstraction is normally made.</font>
> 


> <font size="-1">NOTE: The definition of an 'activity' is normally used
		  for the structural engineering domain, where the activity typically defines no
		  own coordinate system but rather uses the coordinate system of the element on
		  which it acts. Therefore the definition of a location and local coordinate
		  system can be omitted by not assigning a value to <i>ObjectPlacement</i>, in
		  these cases the local coordinate system shall correspond to the local
		  coordinate system of the structural item or building element on which it acts.
		  </font>
>

In addition the _IfcStructuralActivity_ defines the relation needed to associate actions and/or reactions to the _IfcStructuralItem_ to which it applies.

> <font color="#0000FF" size="-1">HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
>