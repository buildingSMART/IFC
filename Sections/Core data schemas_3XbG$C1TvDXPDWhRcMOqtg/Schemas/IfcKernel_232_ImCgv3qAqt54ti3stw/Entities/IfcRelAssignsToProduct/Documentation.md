This objectified relationship&nbsp;_IfcRelAssignsToProduct_ handles the assignment of objects (subtypes of _IfcObject_) to a product (subtypes of _IfcProduct_).

The _Name_ attribute should be used to classify the usage of the _IfcRelAssignsToProduct_ objectified relationship. The following _Name_ values are proposed:

<ul>
  <li>'<strike>Reference</strike>' : Assignment of a
product (via <i>RelatingProduct</i>)
to a spatial structure (via <i>RelatedObjects</i>) to
which it is referenced (in contrary to being contained - which is
handled by <i>IfcRelContainedInSpatialStructure</i>).</li>
  <ul>
    <li><font color="#ff0000"><small>IFC2x
Edition 3 CHANGE &nbsp;The reference of a product within a spatial
structure is now handled by a new relationship object
IfcRelReferencedInSpatialStructure. The <i>IfcRelAssignsToProduct
      </i>shall not be used to represent this relation from
IFC2x3 onwards.<br>
      </small></font><br>
    </li>
  </ul>
  <li>'<strike>Context</strike>' : Assignment of a
context specific
representation, such as of structural members to a different context
representation (with potentially different decomposition breakdown)
such as of building elements&nbsp;for a specific&nbsp;context
specific representation.&nbsp; </li>
  <ul>
    <li><font color="#ff0000"><small>IFC2x
Edition 3 CHANGE &nbsp;The relation of a structural member (as
instance of <i>IfcStructuralMember</i> or its subclasses)
to a physical element&nbsp; (as instance of <i>IfcElement</i>
or its subclasses) is now handled by a new relationship
object <i>IfcRelConnectsStructuralElement</i>. The <i>IfcRelAssignsToProduct
      </i>shall not be used to represent this relation from
IFC2x3 onwards.<br>
      <br>
      </small></font></li>
  </ul>
  <li>'View' : Assignment of a product (via <i>RelatingProduct</i>)
that is decomposed according to a discipline view, to another product
(via <i>RelatedObjects</i>) that is decomposed according
to a different discipline view. An example is the assignment of the
architectural slab to a different decomposition of the pre manufactured
sections of a slab (under a precast concrete discipline view).</li>
</ul>
> <font color="#0000ff" size="-1">HISTORY
New Entity in IFC Release 2x</font>
>