**Definition
from IAI**: A designation by which materials of an element constructed of a number of material layers is known and through which the relative positioning of individual layers can be expressed.

> <font size="-1"> EXAMPLE: A cavity brick wall would be
modeled as <i>IfcMaterialLayerSet</i>
consisting of three <i>IfcMaterialLayer</i>'s:
brick, air cavity and brick.</font>

****Geometry
use****

Each _IfcMaterialLayerSet_ implicitly defines a reference line (MlsBase), to which the start of the first _IfcMaterialLayer_ is aligned. The total thickness of a layer set is calculated from the individual layer thicknesses, the first layer starting from the reference line and following layers being placed on top of the previous (no gaps or overlaps).

![material layer set](figures/IfcMaterialLayerSet.png)