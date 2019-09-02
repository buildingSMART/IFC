An _IfcElementQuantity_ defines a set of derived measures of an element's physical property. Elements could be spatial structure elements (like buildings, storeys, or spaces) or building elements (like walls, slabs, finishes). The _IfcElementQuantity_ gets assigned to the element by using the _IfcRelDefinesByProperties_ relationship.

The optional _MethodOfMeasurement_ attribute defines the code, e.g. from a standard method of measurement, which had been used to calculate the element quantity.

> <small>NOTE The recognizable values for the name and the
        method of measurement attributes have to be agreed upon
        in further agreement documents, such as implementers
        agreements. Some of these agreements might be limited to
        a certain region, to which the method of measurement
        applies.</small>
> 


The name attribute, given at the individual _Quantities_ provides a recognizable semantic meaning of the element quantity. Both information is needed to establish a precise meaning for the measure value. An optional description may be assigned to each of the _Quantities_. All quantities assigned by a single instance of _IfcElementQuantity_ are deemed to have been generated according to the same method of measurement. However several instances of _IfcElementQuantity_ are assignable to an element, thus allowing for an element having quantities generated according to several methods of measurement.

> <small>EXAMPLE1 To exchange the net floor area of spaces
        in the German region (as <i>IfcSpace</i>), the name might
        be 'HNF1' (area of main function type 1), and the method
        of measurement might be accordingly 'DIN277' (German
        industry norm no. 277)</small>
> 


> <small>EXAMPLE2 The same instance of <i>IfcSpace</i> may
        have a different area measure assigned in the German
        region according to a housing regulation, the name would
        be 'Wohnfl&auml;che' and the method of measurement would
        be '2.BV'. It would be attached to the <i>IfcSpace</i> by
        a separate <i>IfcRelDefinesByProperties</i>
        relationship.</small>
> 


The _IfcElementQuantity_ can have the following subtypes of _IfcPhysicalQuantity_ within its SET of _Quantities_, which count for the basis measure types used:

* count measure 
* weight measure 
* length measure 
* area measure 
* volume measure 
* time measure 

> <small><font color="#0000FF">HISTORY New entity in IFC
        Release 2x. NOTE: It replaces the calcXxx attributes used
        in previous IFC Releases.</font></small>
>