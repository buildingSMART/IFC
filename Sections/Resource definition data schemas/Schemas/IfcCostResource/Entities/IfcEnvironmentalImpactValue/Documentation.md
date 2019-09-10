An _IfcEnvironmentalImpactValue_ is an amount or measure of an environmental impact or a value that affects an amount or measure of an environmental impact.

> <font color="#0000FF" size="-1">HISTORY: New entity in IFC
		2x2</font>

### Use Definitions
The _IfcEnvironmentalImpactValue_ contains the value of the environmental impact. For example this could represent the volume of carbon dioxide emission, amount of operational energy or mass of aluminum used in a product.

Each instance of _IfcEnvironmentalImpactValue_ may also have an ImpactType. There are many possible types of environmental impact value that may be identified. To allow for any type of environmental impact value, the _IfcLabel_ datatype is assigned. The following defines some impact types that might be applied:

<table cellpadding="2" cellspacing="2"> 
		<tr> 
		  <td width="209">CO2 emission</td> 
		</tr> 
		<tr> 
		  <td width="209">Embodied energy</td> 
		</tr> 
		<tr> 
		  <td width="209">Mass of aluminium</td> 
		</tr> 
		<tr> 
		  <td width="209">Operational energy</td> 
		</tr> 
		<tr> 
		  <td width="209">Resource</td> 
		</tr> 
		<tr> 
		  <td width="209">Water pollution</td> 
		</tr> 
	 </table>

Where a formal standard is not used, it is recommended that local agreements should be made to define allowable and understandable impact value types within a project or region.