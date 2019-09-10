The _IfcRelCoversBldgElements_ is an objectified relationship between an element and one to many coverings, which cover the building element.

Coverings may be defined primarily as coverings of elements, like an isolation covers a pipe, or as coverings of spaces, as a cladding is often referred to as a space finish.

* _IfcRelCoversBldgElements_, this relationship, expresses the primary relation to the element,
* _IfcRelCoversSpaces_ expresses the primary relation to the space.

> <small><font color="#0000FF">HISTORY New Entity in IFC
      Release 1.5</font></small>

> <small><font color="#FF0000">IFC2x PLATFORM CHANGE: The
      data type of the attribute <i>RelatingElement</i> has been
      changed from <i>IfcBuildingElement</i> to its supertype
      <i>IfcElement</i> with upward compatibility for file based
      exchange. The name <i>IfcRelCoversBldgElements</i> is a known anomaly, 
			as the relationship is not restricted to building elements 
			anymore.</font></small>