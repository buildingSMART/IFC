The _IfcStructuralAnalysisModel_ is used to assemble all information needed to represent a structural analysis model. It encompasses certain general properties (such as analysis type), references to all contained structural members, structural supports or connecting members, the connection properties, as well as loads and the respective load results.

Important functionalities for the description of an analysis model are derived from existing IFC entities:

<ul>
<li><p>From <i>IfcSystem</i>
	it inherits the ability to couple the analysis model via
	<i>IfcRelServicesBuildings</i> to one or more <i>IfcBuilding</i>s as
	necessary.</p>
</li>

<li><p>From <i>IfcGroup</i>
	it inherits the inverse attribute <i>IsGroupedBy</i>, pointing to
	the relationship class <i>IfcRelAssignsToGroup</i>.
	This allows to group structural members
	(instances of <i>IfcStructuralMember</i>), and supports
	(instances of <i>IfcStructuralConnection</i>) which belong
	to a specific analysis model.</p>

	<blockquote>
		<p><font size="-1">NOTE:
		Loads (as instances of <i>IfcStructuralAction</i>)
		are not included through <i>IsGroupedBy</i>. Loads are assigned
		through the <i>LoadedBy</i> attribute relationship, using
		load groups as a grouping mechanism.
		Only top-level load groups should be referenced via <i>LoadedBy</i>.
		</font></p>

		<p><font size="-1">NOTE:
		Results (as instances of <i>IfcStructuralReaction</i>)
		are not included through <i>IsGroupedBy</i>. Results are assigned
		through the <i>HasResults</i> attribute relationship,
		using result groups as a grouping mechanism.</font></p>
	</blockquote>
</li>

<li><p>From <i>IfcObject</i>
	it inherits the inverse attribute <i>IsDecomposedBy</i>
	pointing to the relationship class <i>IfcRelNests</i>. It
	provides the hierarchy between the separate (partial) analysis models.</p>
</li>
</ul>
> <font color="#0000ff" size="-1">HISTORY:
	New entity in Release IFC2x Edition 2.</font>
>