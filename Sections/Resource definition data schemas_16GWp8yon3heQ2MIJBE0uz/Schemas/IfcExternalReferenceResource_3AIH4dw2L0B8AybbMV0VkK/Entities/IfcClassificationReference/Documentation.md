An _IfcClassificationReference_ is a reference into a classification system or source (see _IfcClassification_). An optional inherited _ItemReference_ key is also provided to allow more specific references to classification items (or tables) by type. The inherited _Name_ attribute allows for a human interpretable designation of a classification notation (or code) - see use definition of "Lightweight Classification".

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC
		2x.</font>

### Use Definitions
#### Lightweight Classification
The _IfcClassificationReference_ can be used as a form of 'lightweight' classification through the '_ItemReference_' attribute inherited from the abstract _IfcExternalReference_ class. In this case, the '_ItemReference_' could take (for instance) the Uniclass notation "L6814" which, if the classification was well understood by all parties and was known to be taken from a particular classification source, would be sufficient. The _Name_ attribute could be the title "Tanking". This would remove the need for the overhead of the more complete classification structure of the model.

However, it is not recommended that this lightweight method be used in cases where more than one classification system is in use or where there may be uncertainty as to the origin or meaning of the classification.

#### Referencing from an External Source
Classifications of an object may be referenced from an external source rather than being contained within the IFC model. This is done through the _IfcClassificationReference_ class.