An _IfcExternalReference_ is the identification of information that is not explicitly represented in the current model or in the project database (as an implementation of the current model). Such information may be contained in classifications, documents or libraries.

Only the _Location_ (e.g. as an URL) is given to describe the place where the information can be found. Also an optional _ItemReference_ as a key to allow more specific references (as to sections or tables) is provided. The _ItemReference_ defines a system interpretable method to identify the relevant part of information at the data source (given by _Location_). In addition a human interpretable _Name_ can be assigned to identify the information subject (e.g. classification code).

_IfcExternalReference_ is an abstract supertype of all external reference classes.

> <font color="#0000FF" size="-1">HISTORY: New Class in IFC
		Release 2x to generalize means of referencing available in IFC Release 2.0.
		</font>

### Use Definitions
See the use definitions given at the subtypes of _IfcExternalReference_.