The element type (_IfcDiscreteAccessoryType_) defines a list of commonly shared property set definitions of a discrete accessory and an optional set of product representations. It is used to define a supporting element mainly within structural and building services domains (i.e. the specific type information common to all occurrences of that type).

The occurrences of the _IfcDiscreteAccessoryType_ are represented by instances of _IfcDiscreteAccessory_.

The _IfcDiscreteAccessoryType_ is a specialization of the general building element component type to represent different type of structural and building service related auxiliary elements.

> <font color="#0000FF" size="-1">HISTORY New entity in IFC
		Release 2x2 </font>

**General usage**

The exact type information of the _IfcDiscreteAccessoryType_ is given in the _ElementType_ attribute inherited from _IfcElementType_. Standard type designations are provided for guideline below. The list is not exhaustive and the list of definitions may be extended based on local national extensions.

<table border="1"> 
		<tr> 
		  <td><i><b>Accessory type</b></i></td> 
		  <td><i><b>Standard type designation</b></i></td> 
		  <td><i><b>Description</b></i></td> 
		</tr> 
		<tr> 
		  <td>Shading devices:</td> 
		  <td>'Shading device'</td> 
		  <td>Elements specifically designed to provide shading, often fixed
			 externally and sometimes moving (e.g. by rotation)</td> 
		</tr> 
		<tr> 
		  <td>Corbels as separate components:</td> 
		  <td>'Hidden steel corbel'</td> 
		  <td>Corbel system made from steel components embedded into the master
			 element</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Visible steel corbel'</td> 
		  <td>Corbel system made from steel components protruding from the master
			 element</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Visible concrete corbel'</td> 
		  <td>Corbel system made as a separate precast concrete component added
			 to the master element</td> 
		</tr> 
		<tr> 
		  <td>Anchor bolts:</td> 
		  <td>'Foundation bolt'</td> 
		  <td>Fixture with bolt embedded into concrete structures for securing
			 columns or for machine foundations</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Ribbed bar bolt'</td> 
		  <td>Fixture with bolt and one or several anchoring ribbed
			 (reinforcement) bars embedded into concrete structures for securing columns or
			 for machine foundations. </td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Extension bolt'</td> 
		  <td>Fixture with bolt for extension joints between usually precast
			 elements.</td> 
		</tr> 
		<tr> 
		  <td>Connecting accessories, for example for sandwich wall panels:</td> 
		  <td>'Diagonal truss connector'</td> 
		  <td>A fixing device in truss form with diagonal cross bars holding two
			 precast conrete panels together in a sandwich wall panel.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Ladder truss connector'</td> 
		  <td>A fixing device in truss form with straight cross bars in ladder
			 form holding two precast conrete panels together in a sandwich wall panel.</td>
		  
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Panel suspender'</td> 
		  <td>A straight fixing device holding two precast conrete panels
			 together in a sandwich wall panel.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Bracket'</td> 
		  <td>A bracket for supporting various precast concrete components.</td> 
		</tr> 
		<tr> 
		  <td>Electrical accessories for precast concrete elements:</td> 
		  <td>'Conduit'</td> 
		  <td>Conduit for cabling embedded in element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Electrical box'</td> 
		  <td>Electrical box embedded in element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Double electrical box'</td> 
		  <td>A double electrical box embedded in element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Roof box'</td> 
		  <td>Roof box embedded in element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Junction box'</td> 
		  <td>Junction box embedded in element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Splice'</td> 
		  <td>Splice embedded in element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Protective plug'</td> 
		  <td>Protective plug used in element for protecting electrical
			 accessories during manufacturing, transportation and assembly.</td> 
		</tr> 
		<tr> 
		  <td>Fixing parts:</td> 
		  <td>'Standard fixing plate'</td> 
		  <td>Standard fixing plate.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Edge fixing plate'</td> 
		  <td>Fixing plate attached to the edge of an element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Corner fixing plate'</td> 
		  <td>Fixing plate attached to the corner of an element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Slab fixing plate'</td> 
		  <td>Fixing plate for slabs.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Balcony hinge'</td> 
		  <td>Accessory supporting and fixing balconies.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Frame shoe'</td> 
		  <td>Fixing shoe for frames.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Thermo frame'</td> 
		  <td>Thermo frame.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Column shoe'</td> 
		  <td>Fixing shoe for columns.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Wall shoe'</td> 
		  <td>Fixing shoe for walls.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Fixing socket'</td> 
		  <td>Fixing socket.</td> 
		</tr> 
		<tr> 
		  <td>Joint accessories:</td> 
		  <td>'Neoprene bearing plate'</td> 
		  <td>Rubber plate used as a bearing in, for example, joints between
			 column corbels and beams.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Working joint reinforcement'</td> 
		  <td>Reinforcement accessory used in working joints.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Expansion joint reinforcement'</td> 
		  <td>Reinforcement accessory used in expansion joints.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Ribbed steel bar extension'</td> 
		  <td>Extension accessory made of a ribbed (reinforcement) bar used in
			 joints.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Steel pin bolt'</td> 
		  <td>Pin bolt used to join together, for example, columns and
			 beams.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Concrete dowel'</td> 
		  <td>Dowel pin used in joints.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Concrete groove'</td> 
		  <td>A groove made in a joint.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Steel plate'</td> 
		  <td>A steel plate used as an accessory in a joint.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Wire loop'</td> 
		  <td>A joint connector accessory made from a wire loop.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Steel loop'</td> 
		  <td>A joint connector accessory made from a steel bar loop.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Sealing strip'</td> 
		  <td>A strip sealing the joint.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Sealing compound'</td> 
		  <td>Sealing compound protecting and sealing the joint.</td> 
		</tr> 
		<tr> 
		  <td>Lifting accessories:</td> 
		  <td>'Wire lifting hook'</td> 
		  <td>A lifting aid in the form of a wire loop.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Steel lifting hook'</td> 
		  <td>A lifting aid in the form of a steel bar loop.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Lifting socket'</td> 
		  <td>A lifting aid in the form of a socket.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Steel lifting anchor'</td> 
		  <td>A lifting aid in the form of a steel lifting anchor.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Lifting hole'</td> 
		  <td>A lifting aid in the form of a hole.</td> 
		</tr> 
		<tr> 
		  <td>Accessories mainly used in the building services domain:</td> 
		  <td>'Antivibration'</td> 
		  <td>An isolating device to prevent other elements to be effected by
			 vibrations.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Bracket'</td> 
		  <td>A bracket wich is used to support pipes or cables.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Drop rod'</td> 
		  <td>A length of material providing a hanging support to a bracket. Note
			 that a drop rod is considered to include nuts and washers required for
			 securing.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Duct foot'</td> 
		  <td>A base support used to receive a vertical pipe (BS6100 330 3309 -
			 duct foot).</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Framing'</td> 
		  <td>A frame placed around a penetration to prevent scraping against the
			 building surface or structure.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Grommet'</td> 
		  <td>An element placed within a penetration that seals the penetration
			 for a particular reason.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Rack'</td> 
		  <td>A set of shelving for the purposes of storage that may be
			 freestanding or bolted to a structure.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Safety part'</td> 
		  <td>A part, typically installed in vertical shafts at each level, to
			 ensure safety from falling when entering the shaft.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Sleeve'</td> 
		  <td>A thin barrier placed between a penetration and a penetrating
			 element.</td> 
		</tr> 
		<tr> 
		  <td></td> 
		  <td>'Support section'</td> 
		  <td>A section of material that is used as an intermediate support upon
			 which multiple brackets can be mounted.</td> 
		</tr> 
	 </table>