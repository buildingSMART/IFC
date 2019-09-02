_IfcMaterial_ is a homogeneous or inhomogeneous substance that can be used to form elements (physical products or their components).

_IfcMaterial_ is the basic entity for material designation and definition; this includes identification by name and classification (via reference to an external classification), as well as association of material properties (isotropic or anisotropic) defined by (subtypes of) _IfcMaterialProperties_. An instance of _IfcMaterial_ may be associated to an element or element type using the _IfcRelAssociatesMaterial_ relationship. The assignment might either be direct as a single material information, or via

* a material layer set
* a material profile set
* a material constituent set

An _IfcMaterial_ may also have presentation information associated. Such presentation information is provided by _IfcMaterialDefinitionRepresentation_, associating curve styles, hatching definitions or surface colouring/rendering information to a material.

> HISTORY New entity in IFC4

{ .change-ifc2x4}
> IFC4 CHANGE  The attributes _Description_ and _Category_ have been added.

___
## Common Use Definitions
[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcmaterial.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialCombustion</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialCommon</td></tr>
<tr><td>Concrete</td><td>Pset_MaterialConcrete</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialEnergy</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialFuel</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialHygroscopic</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialMechanical</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialOptical</td></tr>
<tr><td>Steel</td><td>Pset_MaterialSteel</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialThermal</td></tr>
<tr><td>&nbsp;</td><td>Pset_MaterialWater</td></tr>
<tr><td>Wood</td><td>Pset_MaterialWood</td></tr>
<tr><td>Wood</td><td>Pset_MaterialWoodBasedBeam</td></tr>
<tr><td>Wood</td><td>Pset_MaterialWoodBasedPanel</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcMaterial Property Sets for Objects</p></td></tr></table>