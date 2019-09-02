The element type (_IfcFastenerType_) defines a list of commonly shared property set definitions of a fastener and an optional set of product representations. It is used to define fasteners mainly within structural and building services domains (i.e. the specific type information common to all occurrences of that type).

The occurrences of the _IfcFastenerType_ are represented by instances of _IfcFastener_.

> <font color="#0000FF" size="-1">
            HISTORY New entity in IFC Release 2x2
</font>

**General usage**

The exact type information of the _IfcFastenerType_ is given in the _ElementType_ attribute inherited from _IfcElementType_. Standard type designations are provided for guideline below. Note that mechanical fastener types are represented by instances of the subtype _IfcMechanicalFastenerType_.

<table border="1">

   <tr>
       <td><i><b>Standard fastener type designation</b></i></td>
       <td><i><b>Description</b></i></td>
   </tr>
   <tr>
       <td>'Glue'</td>
       <td>A fastening connection where glue is used to join together elements.</td>
   </tr>
   <tr>
       <td>'Weld'</td>
       <td>A weld seam used to join together building elements.</td>
   </tr>
   <tr>
       <td>'Jointing mortar'</td>
       <td>Mortar used to join together building elements.
           The strength of the joint may be taken into consideration in calculations.</td>
   </tr>

</table>