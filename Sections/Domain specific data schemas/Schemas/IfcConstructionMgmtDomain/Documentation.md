The _IfcConstructionMgmtDomain_ schema defines concepts in the construction management (CM) domain. Together with the _IfcProcessExtension_ and _IfcSharedMgmtElement_ schemas it provides a set of models that can be used to exchange information between construction management applications.

## Scope
The _IfcConstructionMgmtDomain_ schema extends the ideas concerning management outlined in the _IfcSharedMgmtElements_ schema. The objective of the _IfcConstructionMgmtDomain_ schema is to capture information that supports specific business processes and resource requirements that are wholly within the domain of interest of the Construction Manager. The aim is to provide support for information exchange and sharing within computer aided management applications. The extent of the model will not support the some of the more detailed ideas found in these applications.

The following are within the scope of this schema:

* resources used in the construction process including product, labor, construction equipment, crew, sub-contract and construction material resources;
* identification of products that result from processes performed that are used as resources in future processes.

## Process Usage
### Resources
Resources are considered to be those things that are used within a process to achieve or assist the process of construction. Various types of resource are defined within the model.

### Product Composition Structure
Construction management activities may take place either on a complete product (the whole), on a part of the product or on a set of products acting as a single product entity (complex). The product composition structure enabling parts, whole, and complexes to be identified is achieved using aggregation or nesting subtype of the _IfcRelDecomposes_ relationship class.

### Products as Resources
A product that results from a process may be used as a resource in a subsequent process.

## Quantity Usage
The quantities of a resource used may be defined therough _IfcRelDefinesByProperties_ using the _IfcElementQuantity_ property set definition
