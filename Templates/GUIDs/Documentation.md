The universal unique identifier standard UUID with its implementation as a globally unique identifier GUID. The generated GUID is compressed for exchange purpose following a&nbsp; compression function published by buildingSMART. The compressed GUID is called "IFC-GUID"

Note: See [buildingsmart-tech.org](http://buildingsmart-tech.org/developers/get-started/ifc-guid){ target="_blank"} for IFC-GUID instructions and examples

The IFC-GUID has to be assigned to the _element_. The following requirements are stipulated by this concept template for all "applicable elements":

*  the IFC-GUID shalI be unique (there shall be never two identical IFC-GUID&#39;s in an IFC data set)
*  the IFC-GUID shall be permanent 
    *  an IFC data set imported into an application shall maintain the imported IFC-GUID&#39;s for all imported elements.
    *  if the same, or modified, IFC data set is exported again from that application, the imported elements (even if modified) shall carry the same IFC-GUID they had on import. 

The **concept template** set as default requirement that "applicable elements" are

*  all subtype of _IfcProduct_,
*  and all subtypes of _IfcTypeProduct_

A **model view definitio**n shall clearly define the "applicable elements" if those differ from the default definition here..