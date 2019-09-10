The element type _IfcPlateType_ defines a list of commonly shared property set definitions of a thin planar element and an optional set of product representations (i.e. the specific product information, that is common to all occurrences of that product type).

> <font size="-1">NOTE&nbsp; The product
representations are defined as representation maps (at the level of the
supertype <i>IfcTypeProduct</i>, which gets assigned by an
element occurrence instance through the <i>IfcShapeRepresentation.Item[1]</i>
being an <i>IfcMappedItem</i>.</font>
> 


A&nbsp;plate type is used to define the common properties of a certain type of a plate that may be applied to many instances of that type to assign a specific style. Plate types may be exchanged without being already assigned to occurrences. It is used to define a planar, or plate-like parts to be located by one or several instances of _IfcPlate_.&nbsp;

The occurrences of the _IfcPlateType_ are represented by instances of _IfcPlate_.

> <font color="#0000ff" size="-1">
HISTORY New entity in IFC
Release 2x2 </font>

**Use definition for steel members**

When using the _IfcPlateType_ as underlying type for steel members in steel construction applications the following additional conventions apply:

**Material association:**  
The _IfcPlateType_ is associated with exactly one instance of _IfcMaterial_ by the _IfcRelAssociatesMaterial_ relationship. This material association assigns a common material to all occurrences (_IfcPlate_) of the _IfcPlateType_. If an individual occurrence has an own material assignment (see _IfcPlate_), then that assignment overrides the material assignment given at the _IfcPlateType_.

**Geometric representation:**  
The plate type must have a full geometric representation, normally given by _IfcExtrudedAreaSolid_. Possibly standardized profile names for the plate have no meaning. The _IfcPlateType_ has (at least) one representation map assigned through the _RepresentationMaps_ relation. The representation map has a full geometric representation given by:

* **Solid:** Only _IfcExtrudedAreaSolid_ shall be supported. 
* **Profile:** Only _IfcArbitraryClosedProfileDef_shall be supported. The profile represents the contour of the plate. 
* **Extrusion:** The extrusion axis shall be perpendicular to the swept profile, i.e. pointing into the direction of the z-axis of the position of the _IfcExtrudedAreaSolid_. Since the profile instance represents the contour of the plate, the extrusion direction corresponds to the plate thickness. 

**Position number:**  
The position number is specified in the attribute _IfcTypeProduct.Tag_.

**Non geometric profile properties:**  
Non geometric profile properties (for instance mechanical properties) are specified through _IfcProfileProperties_ (and its specific subtypes that are related to the cross section). These properties are attached to _IfcPlateType_ by the relationship _IfcRelAssociatesProfileProperties_. If an individual occurrence has an own profile property assignment (see _IfcPlate_), then this assignment overrides the profile property assignment given in _IfcPlateType_.

**Quantity related properties:**  
Quantity related properties,which do not relate to the profile, are specified through _IfcElementQuantity_ (and its specific subtypes). These properties are attached to the _IfcPlateType_ by the relationship _IfcRelDefinesByProperties_. If an individual occurrence has an own element quantity assignment (see _IfcPlate_), then this assignment overrides the quantity assignment given in _IfcPlateType_. The following quantities are foreseen, but will be subjected to the local standard of measurement used:

<table border="1">
  <tbody>
    <tr>
      <td><font size="-1"><i><b>Name</b></i></font></td>
      <td><font size="-1"><i><b>Description</b></i></font></td>
      <td><font size="-1"><i><b>Value
Type</b></i></font></td>
    </tr>
    <tr>
      <td><font size="-1">CrossSectionArea</font></td>
      <td><font size="-1">Total area of the cross
section (or profile) of the
plate (or its basic surface area). The exact definition and calculation
rules
depend on the method of measurement used.</font></td>
      <td><font size="-1"><i>IfcQuantityArea</i></font></td>
    </tr>
    <tr>
      <td><font size="-1">GrossVolume</font></td>
      <td><font size="-1">Total gross volume of the
plate, not taking into
account possible processing features (cut-outs, etc.) or openings and
recesses.
The exact definition and calculation rules depend on the method of
measurement
used.</font></td>
      <td><font size="-1"><i>IfcQuantityVolume</i></font></td>
    </tr>
    <tr>
      <td><font size="-1">NetVolume</font></td>
      <td><font size="-1">Total net volume of the
plate, taking into account
possible processing features (cut-outs, etc.) or openings and recesses.
The
exact definition and calculation rules depend on the method of
measurement
used.</font></td>
      <td><font size="-1"><i>IfcQuantityVolume</i></font></td>
    </tr>
    <tr>
      <td><font size="-1">GrossWeight</font></td>
      <td><font size="-1">Total gross weight of the
plate without add-on
parts, not taking into account possible processing features (cut-outs,
etc.) or
openings and recesses.</font></td>
      <td><font size="-1"><i>IfcQuantityWeight</i></font></td>
    </tr>
    <tr>
      <td><font size="-1">NetWeight</font></td>
      <td><font size="-1">Total net weight of the
plate without add-on parts,
taking into account possible processing features (cut-outs, etc.) or
openings
and recesses.</font></td>
      <td><font size="-1"><i>IfcQuantityWeight</i></font></td>
    </tr>
  </tbody>
</table>
