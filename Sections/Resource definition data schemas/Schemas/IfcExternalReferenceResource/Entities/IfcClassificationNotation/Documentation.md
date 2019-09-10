An _IfcClassificationNotation_ is a notation used from published reference (which may be either publicly available from a classification society or is published locally for the purposes of an organization, project or other purpose).

> <font color="#0000FF" size="-1">HISTORY: New class in IFC
		Release 1.5. It has changed in IFC Release 2x. Documentation corrections made
		in IFC 2x Addendum 1</font>

### Use Definitions
A classification notation may be developed using various notation facets. A facet is a part of the actual notation but which has a specific meaning. For instance, it may be appropriate to classify an item by owning actor (represented by A=Architect) and by an entry from a classification table such as CI/SfB (represented by 210 for external wall). This gives a classification as A210.

All classifications of an object that are contained within the IFC model are made through the _IfcClassificationNotation_ class. For a given object, the _IfcRelAssociatesClassification_ class makes the connection between the _IfcObject_ and the _IfcClassificationNotation_.

It is a requirement that a classification notation can only bring together facets from the same classification system or source. Bringing together notation facets from different sources within the same classification notation is not allowed. However, multiple classifications can be applied to a single object through the use of more than one instance of _IfcRelAssociatesClassification_. In this way it is possible to define multiple classification notations where each notation contains facets from a single source.