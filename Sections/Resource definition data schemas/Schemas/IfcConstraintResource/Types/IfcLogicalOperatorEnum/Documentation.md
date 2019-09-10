_IfcLogicalOperatorEnum_ is an enumeration that defines the logical operators that may be applied for the satisfaction of more than one constraint at a time.

> <font color="#0000FF" size="-1"> HISTORY: New type in IFC Release 2.0.
		  Renamed from IfcConstraintSAggregatorEnum in IFC 2x2 </font>
> 


**Enumeration**

<table border="1"> 
		<tr> 
		  <td><i>Value</i></td> 
		  <td><i>Definition</i></td> 
		</tr> 
		<tr> 
		  <td>LOGICALAND</td> 
		  <td>Defines a relationship between constraints whereby the provisions
			 of all constraints must be satisfied simultaneously (e.g. constraint A AND
			 constraint B must both be satisfied for the constraint as a whole to be
			 satisfied).</td> 
		</tr> 
		<tr> 
		  <td>LOGICALOR</td> 
		  <td>Defines a relationship between constraints whereby the provisions
			 of at least one of the constraints must be satisfied (e.g. constraint A OR
			 constraint B or the provisions of both may be satisfied for the constraint as a
			 whole to be satisfied).</td> 
		</tr> 
	 </table>
