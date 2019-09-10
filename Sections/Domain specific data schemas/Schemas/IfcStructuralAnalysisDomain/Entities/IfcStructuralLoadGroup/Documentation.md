The entity _IfcStructuralLoadGroup_ is used to structure the physical impacts. By using the grouping features inherited from _IfcGroup_, instances of _IfcStructuralAction_ (or its subclasses) and of _IfcStructuralLoadGroup_ can be used to define load groups, load cases and load combinations. An optional coefficient can be provided to represent safety factors known from several codes of practice. (see also _IfcLoadGroupTypeEnum_)

> <font size="-1">NOTE: Important functionality for the description of a
		  load-bearing system is derived from the existing IFC entity <i>IfcGroup</i>.
		  This class provides, via the relationship class <i>IfcRelAssignsToGroup</i>,
		  the needed grouping mechanism. In this way, instances of
		  <i>IfcStructuralAction</i> belonging to a specific load group can be
		  unambiguously determined.</font>
> 


> <font color="#0000FF" size="-1"> HISTORY: New entity in Release IFC2x
		  Edition 2. </font>
> 


U**se Definition**

The following example illustrates the use of this entity class for the different load group types. Common to all these types is the application of the same grouping mechanism (via _IfcGroup_) for the specification of the needed groups that may optionally contain an additional load factor (attribute _Coefficient_). The calculation of internal forces and the provision of safety coefficients is dependent on the building codes used; therefore only a generic representation of load groups is provided by this entity class.

<table width="100%" border="0" cellpadding="0" cellspacing="0"> 
		<tr> 
		  <td><img src="figures/ifcstructuralloadgroup-fig1.gif" alt="Fig. 4-13" width="600" height="316" border="0" align="LEFT"></td> 
		</tr> 
		<tr> 
		  <td height="40" valign="TOP"> 
			 <p>&nbsp;<font size="-1">Example for the definition of load
				cases.</font></p></td> 
		</tr> 
		<tr> 
		  <td><img src="figures/ifcstructuralloadgroup-fig2.gif" alt="Fig. 4-14" width="600" height="350" border="0" align="LEFT"></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" height="40"> 
			 <p>&nbsp;<font size="-1">Example for the definition of load
				combination groups.</font></p></td> 
		</tr> 
		<tr> 
		  <td><img src="figures/ifcstructuralloadgroup-fig3.gif" alt="Fig. 4-15" width="600" height="311" border="0" align="LEFT"></td> 
		</tr> 
		<tr> 
		  <td valign="TOP" height="40"> 
			 <p>&nbsp;<font size="-1">Example for the definition of load
				combinations.</font></p></td> 
		</tr> 
	 </table>
