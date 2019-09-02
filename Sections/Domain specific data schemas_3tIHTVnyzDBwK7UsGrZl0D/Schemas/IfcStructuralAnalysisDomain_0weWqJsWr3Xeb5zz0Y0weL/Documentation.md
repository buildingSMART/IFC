The _IfcStructuralAnalysisDomain_ describes the structural analysis model in order to tightly integrate the structural engineering domain. It reuses the existing building element and spatial structure element definition and associates the structural assumptions to it. The focus is to ensure that structural engineering information is captures and made visible to other related domains.

The following features are in scope:

* Defining planar and/or spatial structural analysis models which can be used by structural analysis applications.
* Included are, basically: 
    *  point, line and planar structural elements as well as supports 
    * their connectivity and support conditions. 
    *  Specification of loadings including point, line planar and temperature loads and the assignment to load groups, load cases and load combinations. 
    *  Specification of different structural analysis models which is needed to describe different aspects or parts of the building. Furthermore, dependencies between these models can be stored in the model for further use. 
    *  Analysis results defined by force and displacement.
Currently not in scope are:

* Dynamic analysis 
*  Description of prestressed loads 
*  Finite element topology 
*  Detailed results in finite element meshes as well as stresses and strains in the structural elements. 

> <font size="-1" color="#0000FF">HISTORY: New schema in Release
		IFC2x Edition 2.</font>