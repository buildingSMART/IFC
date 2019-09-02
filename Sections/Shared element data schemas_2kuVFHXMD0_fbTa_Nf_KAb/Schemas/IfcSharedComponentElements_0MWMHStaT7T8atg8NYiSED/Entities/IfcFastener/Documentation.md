Representations of fixing parts which are used as fasteners to connect or join elements with other elements.

> <font color="#0000FF" size="-1">
   HISTORY New entity in IFC Release 2x2
</font>

**General usage**

The exact type information of the _IfcFastener_ is given in the _ObjectType_ attribute inherited from _IfcObject_. Standard type designations are provided for guideline below. Note that mechanical fasteners are represented by instances of the subtype _IfcMechanicalFastener_.

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

**Geometry Use Definitions:**

The geometric representation of _IfcFastener_ is given by the _IfcProductDefinitionShape_, allowing multiple geometric representations. Included are:

**Local Placement**  
The use of local placement is defined in the supertype _IfcElementComponent_.

**Standard Geometric Representation**  
The use of Standard Geometric Representations is defined in the supertype _IfcElementComponent_.