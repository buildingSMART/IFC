**Definition
from IAI:** The abstract entity _IfcStructuralMember_ is the superclass of all structural elements representing the structural behavior of building elements. A further differentiation is made for structural curve members and structural face members (see _IfcStructuralCurveMember_ and _IfcStructuralFaceMember_). Structural members can have&nbsp;

* a material definition, using _IfcStructuralMember o-- IfcRelAssociatesMaterial --o IfcMaterial_
* a profile definition, using _IfcStructuralMember o-- IRelAssociatesProfileProperties --o IfcProfileProperties_
* a parent analysis model, using _IfcStructuralMember o-- IfcRelAssignsToGroup --o IfcStructuralAnalysisModel_

> <font size="-1">NOTE: Currently only the subtypes <i>IfcStructuralCurveMember</i>
and <i>IfcStructuralFaceMember</i>
are defined. However, for dynamic calculations, an extension for 'point
members' will be necessary and might be added in future releases.</font>
> 


> <font color="#0000ff" size="-1">HISTORY: New entity
in Release IFC2x Edition 2. </font>
> 


****Use
Definition****

<table border="0" cellpadding="0" cellspacing="0" width="100%">
  <tbody>
    <tr>
      <td><img alt="material" src="figures/ifcstructuralmember-fig1.gif" height="240" width="500"><br>
      </td>
      <td valign="top"><small><i>Assignment
of Material </i><br>
The relationship to a specific material definition is provided by the
entity class <i>IfcRelAssociatesMaterial</i>.
The instance of <i>IfcStructuralMember</i>
is used to represent collectively its subclasses <i>IfcStructuralCurveMember</i>
and <i>IfcStructuralFaceMember</i>.<br>
      </small><br>
      <font size="-1">Depending
on the material, there are material specific subtypes of <i>IfcMechanicalMaterialProperties</i>,
such as <i>IfcMechanicalSteelMaterialProperties</i>,
or <i>IfcMechanicalConcreteMaterialProperties</i>.</font></td>
    </tr>
    <tr>
      <td height="40" valign="top">
      <p>&nbsp;<img alt="analysis model" src="figures/ifcstructuralmember-fig2.gif" height="250" width="250"><font size="-1"><br>
      </font></p>
      </td>
      <td valign="top"><small><i>Structural
analysis model for structural members</i><br>
Assignment of structural members to a structural analysis model.</small></td>
    </tr>
  </tbody>
</table>