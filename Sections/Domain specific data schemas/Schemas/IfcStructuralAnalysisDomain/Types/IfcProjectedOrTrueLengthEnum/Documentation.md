This enumeration type is needed for load definition and is only considered if the load values are given as global actions and if they define linear or planar loads.

The _IfcProjectedOrTrueLengthEnum_ type is referenced by the entity _IfcStructuralAction_ and its respective subclasses. It also depends on the attribute value_GlobalOrLocal_ of supertype _IfcStructuralActivity_ and should only take effect if _GlobalOrLocal_ is set to GLOBAL_COORDS.

> <font color="#0000FF" size="-1">HISTORY: New type in Release IFC2x
		  Edition 2. </font>
> 


!["projected or true length"](../../../../../../figures/ifcprojectedortruelengthenum-fig1.gif "<font size="-1">Fig. 4-5<br>Illustration of the different
				interpretation of a load definition depending on the enumeration types
				<i>IfcGlobalOrLocalEnum</i> and
				<i>IfcProjectedOrTrueLengthEnum</i></font>")
