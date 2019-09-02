The IfcExternalReferenceResource supports the reference to external sources of information. Currently three sources of external information are handled:

* Classifications
* Documents
* Libraries

The following overview is given for those concepts separately.

## Classification
### Introduction
The Classification model in IFC has developed progressively from its introduction within version 1.0 of the specification. Initially based on work undertaken for the ISO 10303 part 106 (Building Construction Core Model) in conjunction with ISO Technical Committee 59, it has been extensively redeveloped in conjunction with classification experts for use by the IFC 2x specifications.

The Classification model in IFC recognizes that there are many different classification systems in use throughout the AEC/FM industry and that their use differs according to geographical location, industry discipline and other factors. For a generic model such as IFC, it is necessary to allow for the adoption of any rational classification system whether it be based on elements, work sections or any other classifiable division.

The Classification model in IFC is able to represent classifications according to the most advanced current concepts from work in ISO, ICIS (International Construction Information Society) and EPIC (European Product Information Coding) as well as more traditional classifications such as those in the various SfB forms used internationally, CAWS, Masterformat etc.

### Scope
The Classification model in IFC forms part of the _IfcExternalReferenceResource_ schema and specifies the use of the independent resources necessary for the scope and information requirements for the exchange and sharing of classification information between application systems. Such information may be used at all stages of the life-cycle of a building

The following are within the scope of this part of the specifications:

* The provision of one or more classification notations to an object.
* The inclusion of one or more facets to a classification notation.
* Referencing of facets of a classification notation from a described source (classification item or classification table)
* Exposure of the hierarchy of a classification structure.
* Identification of the source of the classification.
* The designation of a classification in terms of its source, edition and name. 
* The provision of a means of semantically identifying the meaning of a classification notation.
* Referencing a classification held on an external source.

The following are outside of the scope of this part of the specifications:

* The ability to translate from one classification notation to another.

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td width="41"><a href="lexical/text/ClassificationUsage.htm" target="SOURCE"><img src="lexical/text/img/go.gif" alt="go" width="38" height="20" border="0"></a></td> 
		  <td bgcolor="#C8C8C8">see attached document for more on classification usage</td> 
		</tr> 
	 </table>

  
___
## Documents
The IFC Documents Model enables reference to be made to documents stored externally to a populated IFC model or for information about documents to be stored within the model.

### Scope
The scope of the IFC Documents Model is:

*  to manage reference to documents
* to manage information about documents
* to be equally applicable to documents that are paper based or stored electronically

The IFC Documents Model is not designed to be a complete document model and does not overlap in intent or content with such models.

For details about such models, attention is drawn to the Document Object Model (DOM) issued by the World Wide Web Consortium which can be obtained from their web site at http://www.w3c.org.

#### Referencing External Documents
The IFC Documents Model considers that information may well be referenced from external sources. Reference a document is by its location (address) to enable access through mechanisms such as the World Wide Web. This is done through the IfcDocumentReference class. This is a type of IfcExternalReference that has a label (which can be the reference address) and identifier. Additionally, a name attribute provides the document with a human readable extension or qualifier to the location.

Optionally, as well as the document reference itself, information concerning the document can also be stored as an attribute of the document reference.

#### Document Information
Information about a document (sometimes referred to as metadata) can be held using the _IfcDocumentInformation_ class. This identifies and names the document, names the document owner and, optionally, can include a description of the document. Additionally, a revision identifier for the document may also be included.

Document information can also include creation and revision times and the duration of its validity by reference to 'valid from' and 'valid to' attributes.

For a document that is stored electronically, the _IfcElectronicDocumentFormat_ class enables information about the format to be recorded. This includes the file extension used and information about the content using the MIME standard.

#### Document Information Relationships
Documents frequently hold references to information held in other documents e.g. documents referencing standards that are also documents. A significant tree structure of document information referencing could be built up in this way. Such relationships between document information can be captured through the _IfcDocumentInformationRelationship_ class which manages both relating and related document information and inversely captures the document information carrying the pointer and the document information to which pointers refer.

___
## Library References
The ability to reference product information stored in external data libraries was introduced in IFC Release 2.0. In IFC 2x, the model has been further developed based on review and pilot testing of the model. This has resulted in moving the IFC Libraries Model from a being a subtype of IfcProperty to being a resource in its own right within the _IfcExternalReferenceResource_ schema.

The rationale of the IFC Libraries Model is that much of the information that will be used to populate a model exists in external data sources. While this can be brought into the model through objects and property sets, it may well be best to simply keep a reference to the location from where it can be obtained and leave it there. This has the potential advantage that, when required, the information from the library will be up to date having been maintained by the library provider. This may not be the case if the information is used to populate the model immediately.

It also has the advantage that the volume of information within the model is kept to a minimum. For file exchange, this can be used effectively to delegate the actual acquisition of information to populate the model to the most appropriate source (providing they have access to the library referenced) rather than the first user having to acquire the information.

#### Scope
The scope of the IFC Libraries Model is to be able to reference information stored in external data libraries.

The following are out of scope of the IFC Libraries Model:

* the format in which data are stored within the external data source
* the format in which data may be retrieved and transported from the external data source to populate an IFC model.
* the means by which transported information populates an IFC model.

#### Assumption
It is assumed that, most frequently, information will populate property sets within an IFC model and that many of these property sets will be defined outside of the formal development mechanisms of the IAI.

Attention is drawn to the IfcPropertyResourceSchema and particularly to the IfcExtensionPropertySet class which has an optional LibraryReference attribute.

#### Library Referencing
As well as the IfcLibraryReference which contains a fully qualified location, reference and further qualification identifier (inherited from the IfcExternalReferenceResource class), the IfcLibraryInformation class specifies further detail about the library from which the information may be obtained. This includes the name of the library and optionally, its publisher, version number and version date.