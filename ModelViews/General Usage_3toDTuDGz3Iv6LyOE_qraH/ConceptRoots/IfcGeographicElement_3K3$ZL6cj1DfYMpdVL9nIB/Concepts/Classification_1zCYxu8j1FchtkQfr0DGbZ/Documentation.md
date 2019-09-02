An _IfcGeographicElement_ might be further qualified by referencing a feature catalog as a particular classification. The feature classification is assigned using the inverse relationship _HasAssociations_ pointing to _IfcClassificationReference_. The attributes should have the following meaning:

* Catalog : _IfcClassification.Name_ 
* Identity: _IfcClassificationReference.Identification_ 
* ElementName: _IfcClassificationReference.Name_