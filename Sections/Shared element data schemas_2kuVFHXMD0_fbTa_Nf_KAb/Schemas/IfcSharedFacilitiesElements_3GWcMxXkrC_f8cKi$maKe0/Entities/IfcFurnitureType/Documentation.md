An _IfcFurnitureType_ defines a particular type of item of furniture such as a table, desk, chair, filing cabinet etc.

> <font color="#0000ff" size="-1">HISTORY
New entity in IFC 2x2. </font>

**Use Definitions**

An _IfcFurnitureType_ provides for all forms of unit furniture. Refer to description for _IfcSystemFurnitureElementType_ for descriptions of system elements that may be provided as part of a kit or 'flatpack' for local assembly.

Occurrences of a type of furniture are specified through _IfcFurnishingElement_.

****Property Set Use Definition****:

The property sets relating to an _IfcFurnitureType_are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByType_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to an _IfcFurnitureType_ are part of this IFC release:

* [Pset_FurnitureTypeCommon](../../psd/IfcSharedFacilitiesElements/Pset_FurnitureTypeCommon.xml): property set for the properties common to all types of furniture, if available 
* [Pset_FurnitureTypeChair](../../psd/IfcSharedFacilitiesElements/Pset_FurnitureTypeChair.xml): specific property set for the properties of a chair, if available 
* [Pset_FurnitureTypeDesk](../../psd/IfcSharedFacilitiesElements/Pset_FurnitureTypeDesk.xml): specific property set for the properties of a desk, if available 
* [Pset_FurnitureTypeFileCabinet](../../psd/IfcSharedFacilitiesElements/Pset_FurnitureTypeFileCabinet.xml): specific property set for the properties of a filing cabinet, if available 
* [Pset_FurnitureTypeTable](../../psd/IfcSharedFacilitiesElements/Pset_FurnitureTypeTable.xml): specific property set for the properties of a table, if available 

****Geometry Use Definitions****

Representations of the type are defined as representation maps (at the level of the supertype _IfcTypeProduct_). These are assigned at the occurrence through the _IfcShapeRepresentation.Item_ being an _IfcMappedItem_.

****Name Use Definitions****

The name of the type of furniture is defined through the _IfcFurnitureType.Name_ attribute (through inheritance from _IfcRoot_). The following items are examples of names that may be given to instances of _IfcFurnitureType_. It is concerned only with internal furniture. The list is drawn from the Uniclass classification system published by RIBA Enterprises Ltd and is reproduced by permission.

<table>
  <tbody>
    <tr>
      <td>
      <table>
        <tbody>
          <tr>
            <td valign="top" width="210">Wardrobe</td>
          </tr>
          <tr>
            <td valign="top" width="210">Chests of
drawers</td>
          </tr>
          <tr>
            <td valign="top" width="210">Locker</td>
          </tr>
          <tr>
            <td valign="top" width="210">Coat rack</td>
          </tr>
          <tr>
            <td valign="top" width="210">Hatstand</td>
          </tr>
          <tr>
            <td valign="top" width="210">Shoe tree</td>
          </tr>
          <tr>
            <td valign="top" width="210">Cloakroom
unit</td>
          </tr>
          <tr>
            <td valign="top" width="210">Umbrella
stand</td>
          </tr>
          <tr>
            <td valign="top" width="210">Clothes
drying cabinet</td>
          </tr>
          <tr>
            <td valign="top" width="210">Table</td>
          </tr>
          <tr>
            <td valign="top" width="210">Coffee
table</td>
          </tr>
          <tr>
            <td valign="top" width="210">Dining
table</td>
          </tr>
          <tr>
            <td valign="top" width="210">Chair</td>
          </tr>
          <tr>
            <td valign="top" width="210">Easy chair</td>
          </tr>
          <tr>
            <td valign="top" width="210">Settee</td>
          </tr>
          <tr>
            <td valign="top" width="210">Stool</td>
          </tr>
          <tr>
            <td valign="top" width="210">Bench</td>
          </tr>
          <tr>
            <td valign="top" width="210">Chaise
longue</td>
          </tr>
          <tr>
            <td valign="top" width="210">Chair bed</td>
          </tr>
          <tr>
            <td valign="top" width="210">Futon</td>
          </tr>
          <tr>
            <td valign="top" width="210">Sofa bed</td>
          </tr>
          <tr>
            <td valign="top" width="210">Bed</td>
          </tr>
          <tr>
            <td valign="top" width="210">Foldaway
bed</td>
          </tr>
          <tr>
            <td valign="top" width="210">Bunk bed</td>
          </tr>
          <tr>
            <td valign="top" width="210">Divan</td>
          </tr>
          <tr>
            <td valign="top" width="210">Waterbed</td>
          </tr>
          <tr>
            <td valign="top" width="210">Headboard</td>
          </tr>
          <tr>
            <td valign="top" width="210">Cradle</td>
          </tr>
          <tr>
            <td valign="top" width="210">Cot</td>
          </tr>
          <tr>
            <td valign="top" width="210">Bedside
unit</td>
          </tr>
          <tr>
            <td valign="top" width="210">Dressing
table</td>
          </tr>
        </tbody>
      </table>
      </td>
      <td valign="top">
      <table>
        <tbody>
          <tr valign="top">
            <td valign="top" width="253">Bathroom
cabinet</td>
          </tr>
          <tr>
            <td valign="top" width="253">Towel
dispenser</td>
          </tr>
          <tr>
            <td valign="top" width="253">Sanitary
product dispenser</td>
          </tr>
          <tr>
            <td valign="top" width="253">Towel rail</td>
          </tr>
          <tr>
            <td valign="top" width="253">Soap
dispenser</td>
          </tr>
          <tr>
            <td valign="top" width="253">Soap holder</td>
          </tr>
          <tr>
            <td valign="top" width="253">Cupboard</td>
          </tr>
          <tr>
            <td valign="top" width="253">Chest</td>
          </tr>
          <tr>
            <td valign="top" width="253">Sideboard</td>
          </tr>
          <tr>
            <td valign="top" width="253">Dresser</td>
          </tr>
          <tr>
            <td valign="top" width="253">Filing
cabinet</td>
          </tr>
          <tr>
            <td valign="top" width="253">Map chest</td>
          </tr>
          <tr>
            <td valign="top" width="253">Plan chest</td>
          </tr>
          <tr>
            <td valign="top" width="253">Desk tidy</td>
          </tr>
          <tr>
            <td valign="top" width="253">Carousels</td>
          </tr>
          <tr>
            <td valign="top" width="253">Vertical
carousels</td>
          </tr>
          <tr>
            <td valign="top" width="253">Horizontal
carousels</td>
          </tr>
          <tr>
            <td valign="top" width="253">Trolleys</td>
          </tr>
          <tr>
            <td valign="top" width="253">Waste
paper bin</td>
          </tr>
          <tr>
            <td valign="top" width="253">Ashtray</td>
          </tr>
          <tr>
            <td valign="top" width="253">Refuse bag
holder</td>
          </tr>
          <tr>
            <td valign="top" width="253">Fender</td>
          </tr>
          <tr>
            <td valign="top" width="253">Fire hood</td>
          </tr>
          <tr>
            <td valign="top" width="253">Kitchen
cupboard</td>
          </tr>
          <tr>
            <td valign="top" width="253">Worktop</td>
          </tr>
          <tr>
            <td valign="top" width="253">Bottle rack</td>
          </tr>
        </tbody>
      </table>
      </td>
      <td valign="top">
      <table>
        <tbody>
          <tr>
            <td valign="top" width="255">Lectern</td>
          </tr>
          <tr>
            <td valign="top" width="255">Pulpit</td>
          </tr>
          <tr>
            <td valign="top" width="255">Choir
screen</td>
          </tr>
          <tr>
            <td valign="top" width="255">Organ</td>
          </tr>
          <tr>
            <td valign="top" width="255">Font</td>
          </tr>
          <tr>
            <td valign="top" width="255">Showcase</td>
          </tr>
          <tr>
            <td valign="top" width="255">Notice
board</td>
          </tr>
          <tr>
            <td valign="top" width="255">Pin board</td>
          </tr>
          <tr>
            <td valign="top" width="255">Writing
board</td>
          </tr>
          <tr>
            <td valign="top" width="255">Blackboard</td>
          </tr>
          <tr>
            <td valign="top" width="255">Dry marker
board</td>
          </tr>
          <tr>
            <td valign="top" width="255">Poster
display unit</td>
          </tr>
          <tr>
            <td valign="top" width="255">Indoor
poster display unit</td>
          </tr>
          <tr>
            <td valign="top" width="255">Outdoor
poster display units</td>
          </tr>
          <tr>
            <td valign="top" width="255">Information
sign</td>
          </tr>
          <tr>
            <td valign="top" width="255">Nameplate</td>
          </tr>
          <tr>
            <td valign="top" width="255">Plaque</td>
          </tr>
          <tr>
            <td valign="top" width="255">Scoreboard</td>
          </tr>
          <tr>
            <td valign="top" width="255">Consulting
couch</td>
          </tr>
          <tr>
            <td valign="top" width="255">Hospital
bed</td>
          </tr>
          <tr>
            <td valign="top" width="255">Hospital
bedhead</td>
          </tr>
          <tr>
            <td valign="top" width="255">Dissection
table</td>
          </tr>
          <tr>
            <td valign="top" width="255">Post-mortem
table</td>
          </tr>
        </tbody>
      </table>
      </td>
      <td valign="top">
      <table>
        <tbody>
          <tr>
            <td valign="top" width="212">Reception
desk</td>
          </tr>
          <tr>
            <td valign="top" width="212">Footrest</td>
          </tr>
          <tr>
            <td valign="top" width="212">Armrest</td>
          </tr>
          <tr>
            <td valign="top" width="212">Copyholder</td>
          </tr>
          <tr>
            <td valign="top" width="212">Anti-bandit
screen</td>
          </tr>
          <tr>
            <td valign="top" width="212">Safe</td>
          </tr>
          <tr>
            <td valign="top" width="212">Point of
sale unit</td>
          </tr>
          <tr>
            <td valign="top" width="212">Key
security cabinet</td>
          </tr>
          <tr>
            <td valign="top" width="212">Post box</td>
          </tr>
          <tr>
            <td valign="top" width="212">Postroom
rack</td>
          </tr>
          <tr>
            <td valign="top" width="212">Acoustic
hood</td>
          </tr>
          <tr>
            <td valign="top" width="212">Curtain
pelmets</td>
          </tr>
          <tr>
            <td valign="top" width="212">Beanbag</td>
          </tr>
          <tr>
            <td valign="top" width="212">Cushion</td>
          </tr>
          <tr>
            <td valign="top" width="212">Planter</td>
          </tr>
          <tr>
            <td valign="top" width="212">Vase</td>
          </tr>
          <tr>
            <td valign="top" width="212">Plant</td>
          </tr>
          <tr>
            <td valign="top" width="212">Artificial
plant</td>
          </tr>
          <tr>
            <td valign="top" width="212">Ornament</td>
          </tr>
          <tr>
            <td valign="top" width="212">Mirror</td>
          </tr>
          <tr>
            <td valign="top" width="212">Ornamental
screen</td>
          </tr>
          <tr>
            <td valign="top" width="212">Mural</td>
          </tr>
          <tr>
            <td valign="top" width="212">Painting</td>
          </tr>
          <tr>
            <td valign="top" width="212">Print</td>
          </tr>
          <tr>
            <td valign="top" width="212">Sculpture</td>
          </tr>
          <tr>
            <td valign="top" width="212">Clock</td>
          </tr>
          <tr>
            <td valign="top" width="212">Wallhanging</td>
          </tr>
          <tr>
            <td valign="top" width="212">Tapestry</td>
          </tr>
        </tbody>
      </table>
      </td>
    </tr>
  </tbody>
</table>

A similar list could also be defined for external furniture.

Note that the list does not contain any items that have an electrical or other services connection. Generally, these are dealt with under a relevant building services entity e.g. _IfcElectricalApplianceType_.