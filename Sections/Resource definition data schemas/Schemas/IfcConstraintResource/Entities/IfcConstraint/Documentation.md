An _IfcConstraint_ is used to define a constraint or limiting value or boundary condition that may be applied to an object or to the value of a property.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC Release
		  2.0</font>
>

### Use Definition
_IfcConstraint_ may be associated with any subtype of _IfcObject_ through the _IfcRelAssociatesConstraint_ relationship in the _IfcControlExtension_ schema.

A constraint may aggregate other constraints through the _IfcConstraintAggregationRelationship_ through which a logical association between constraints may be applied.

A constraint must have a name applied through the _IfcConstraint.Name_ attribute and optionally, a description through _IfcConstraint.Description_. For instance, when undertaking a move (instantiated through the _IfcMove_ class), a constraint may be named as a 'Move Start Constraint' or 'Move End Constraint' and described using one of a possible range of move constraints as shown in the table below.

<font color="#FF0000">Application of constraints to moves as indicated
		by this example replaces the use of IfcActionTimeControl class which is now
		deleted.</font>

<table border="1"> 
		<tr> 
		  <td><i>Constraint Description</i></td> 
		  <td width="440"><i> Definition</i></td> 
		  <td width="270"><i> Benchmark</i></td> 
		  <td width="100"><i> Grade</i></td> 
		</tr> 
		<tr> 
		  <td>ASSOONASPOSSIBLE</td> 
		  <td width="440">Action should commence at the earliest possible
			 opportunity.</td> 
		  <td width="270">GREATERTHANOREQUALTO</td> 
		  <td width="100">SOFT</td> 
		</tr> 
		<tr> 
		  <td>MUSTSTARTON</td> 
		  <td width="440">Action must start at a prescribed date/time.</td> 
		  <td width="270">EQUALTO</td> 
		  <td width="100">HARD</td> 
		</tr> 
		<tr> 
		  <td>MUSTSTARTBEFORE</td> 
		  <td width="440">Action must start before a prescribed date/time.</td> 
		  <td width="270">LESSTHANOREQUALTO</td> 
		  <td width="100">HARD</td> 
		</tr> 
		<tr> 
		  <td>MUSTSTARTAFTER</td> 
		  <td width="440">Action must not start before a prescribed
			 date/time.</td> 
		  <td width="270">GREATERTHANOREQUALTO</td> 
		  <td width="100">HARD</td> 
		</tr> 
		<tr> 
		  <td>MAYSTARTAFTER</td> 
		  <td width="440">Action may start at any time following a prescribed
			 date/time.</td> 
		  <td width="270">GREATERTHANOREQUALTO</td> 
		  <td width="100">SOFT</td> 
		</tr> 
		<tr> 
		  <td>MUSTFINISHON</td> 
		  <td width="440">Action must be complete at or by a prescribed
			 date/time.</td> 
		  <td width="270">EQUALTO</td> 
		  <td width="100">HARD</td> 
		</tr> 
		<tr> 
		  <td>MUSTFINISHBEFORE</td> 
		  <td width="440">Action must be complete before a prescribed
			 date/time.</td> 
		  <td width="270">LESSTHANOREQUALTO</td> 
		  <td width="100">HARD</td> 
		</tr> 
	 </table>

The constraint is instantiated as the class _IfcMetric_ and uses a Date/Time value through _IfcMetricValue_. An appropriate benchmark is applied according to the requirement of the constraint (as indicated). The grade of the constraint (hard, soft, advisory) must be specified through _IfcConstraint.ConstraintGrade_ whilst the time at which the constraint is created may be optionally asserted through _IfcConstraint.ConstraintTime_.