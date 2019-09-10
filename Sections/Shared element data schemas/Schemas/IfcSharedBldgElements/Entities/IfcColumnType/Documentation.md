The element type _IfcColumnType_ defines commonly shared information for occurrences of columns. The set of shared information may include:

* common properties within shared property sets
* common material information
* common profile definitions
* common shape representations

It is used to define a column specification, or column style (i.e. the specific product information that is common to all occurrences of that column type). Column types may be exchanged without being already assigned to occurrences.

Occurrences of the _IfcColumnType_ within building models are represented by instances of _IfcColumnStandardCase_ if the _IfcColumnType_ has a single associated _IfcMaterialProfileSet_; otherwise they are represented by instances of _IfcColumn_. Occurrences of the _IfcColumnType_ within structural analysis models are represented by instances of _IfcStructuralCurveMember_, or its applicable subtypes.

> HISTORY&nbsp; New entity in IFC2x2.

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifccolumntype.htm)

{ .use-head}
Material Profile Set

The [Material Profile Set](../../templates/material-profile-set.htm) concept applies to this entity.

The material of the _IfcColumnType_ is defined by the _IfcMaterialProfileSet_ or as fall back by _IfcMaterial_ and attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship.

> NOTE&nbsp; It is illegal to assign an _IfcMaterial_ to an _IfcColumnType_, if there is at least one occurrences of _IfcColumnStandardCase_ for this type.

The shared profile definition is defined by assigning an _IfcMaterialProfileSet_ (see material use definition above). The _IfcMaterialProfile_ refers to the subtype of _IfcProfileDef_ that is the common profile for all column occurrence, if used. It is only applicable if the _IfcColumnType_ has only occurrences of type _IfcColumnStandardCase_ (see definition of _IfcColumnStandardCase_ for further information).

> NOTE&nbsp; The attribute _ProfileName_ of the _IfcProfileDef_ subtype, referenced in _IfcMaterialProfile_ should contain a standardized profile name according to local standards. However, an additional geometric representation of the profile is necessary (e.g. as _IfcExtrudedAreaSolid_). An importing application is allowed to check for the existence of the profile name: in case of identifying it as a standardized name, the corresponding profile geometry and possibly other cross sectional properties can be read from a library. Otherwise the geometric representation and possible non geometric _IfcProfileProperties_ have to be used.

  
  
{ .use-head}
Type Body Geometry

The [Type Body Geometry](../../templates/type-body-geometry.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>RepresentationType</b></th><th><b>Geometry</b></th></tr>
<tr><td>SweptSolid</td><td><a href="../../ifcgeometricmodelresource/lexical/ifcextrudedareasolid.htm">IfcExtrudedAreaSolid</a></td></tr>
<tr><td>Brep</td><td><a href="../../ifcgeometricmodelresource/lexical/ifcfacetedbrep.htm">IfcFacetedBrep</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcColumnType Type Body Geometry</p></td></tr></table>

The _IfcColumnType_ may define the shared geometric representation for all column occurrences. The _RepresentationMaps_ attribute refers to a list of _IfcRepresentationMap_'s, that allow for multiple geometric representations (e.g. with _IfcShapeRepresentation_'s having an _RepresentationIdentifier_ 'Box', 'Axis', or 'Body'). It is only applicable if the _IfcColumnType_ has only occurrences of type _IfcColumn_ (See geometric use definition of _IfcColumn_ for further information).

> NOTE&nbsp; If the _IfcColumnType_ has an associated _IfcMaterialProfileSet_, then no shared geometric representation shall be provided.

> NOTE&nbsp; The product shape representations are defined as _RepresentationMaps_ (attribute of the supertype _IfcTypeProduct_), which get assigned by an element occurrence instance through the _IfcShapeRepresentation.Item[n]_ being an _IfcMappedItem_. See _IfcTypeProduct_ for further information.

> NOTE&nbsp; The values of attributes _RepresentationIdentifier_ and _RepresentationType_ of _IfcShapeRepresentation_ are restricted in the same way as those for _IfcColumn_ and _IfcColumnStandardCase_