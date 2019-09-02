An _IfcObjectDefinition_ is the generalization of any semantically treated thing or process, either being a type or an occurrences. Object defintions can be named, using the inherited _Name_ attribute, which should be a user recognizable label for the object occurrance. Further explanations to the object can be given using the inherited _Description_ attribute. A context is a specific kind of object definition as it provides the project or library context in which object types and object occurrences are defined.

Objects are independent pieces of information that might contain or reference other pieces of information. There are four essential kinds of relationships in which object definitons (by their instantiable subtypes) can be involved:

<ul>
<li><b>Assignment of other objects</b> - an assignment relationship
(<em>IfcRelAssigns</em>) that refers to other types of objects and
creates a bi-directional association. The semantic of the
assignment is established at the level of the subtypes of the
general <em>IfcRelAssigns</em> relationship. There is no dependency
implied a priori by the assignment.</li>
<li><b>Association to external resources</b> - an association
relationship (<em>IfcRelAssociates</em>) that refers to external
sources of information (most notably a classification or document)
and creates a uni-directional association. There is no dependency
implied by the association.</li>
<li><b>Aggregation of other objects</b> - an aggregation
relationship (<em>IfcRelAggregates</em>) that establishes an
unordered, spatial whole/part relation and creates a bi-directional
relation. There is an implied dependency established.</li>
<li><b>Nesting of other objects</b> - a nesting relationship
(<em>IfcRelNests</em>) that establishes an ordered, non-spatial
whole/part relation and creates a bi-directional relation. There is
an implied dependency established.</li>
<li><b>Declaration within a context</b> - a relationship
(<em>IfcRelDeclares</em>) of the uppermost object definition within
the object definition tree (e.g. the summary object within an
object nesting tree) to the context (a project or project library).
It applies the units, representation context and other context
information to this object definition and all dependent ones.
<ul>
<li style="list-type-type:none"><small>EXCEPTION&nbsp; The link
between the uppermost object in the spatial structure tree, that is
<em>IfcSite</em> or <em>ifcBuilding</em>, and the context provided
by <em>IfcProject</em> is created using the
<em>IfcRelAggregates</em> relationship. See <em>IfcProject</em> for
more information.</small></li>
</ul>
</li>
</ul>
> HISTORY&nbsp; New abstract entity in IFC2x3.

{ .change-ifc2x4}
> IFC4 CHANGE The new subtype _IfcContext_ and the relationship to context _HasContext_ has been added . The decomposition relationship is split into ordered nesting (_Nests_, _IsNestedBy_) and un-ordered aggregating (_Decomposes_, _IsDecomposedBy_).