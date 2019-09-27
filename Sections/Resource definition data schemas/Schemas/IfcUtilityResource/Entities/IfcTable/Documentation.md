﻿An _IfcTable_ is a data structure for the provision of information in the form of rows and columns. Each instance may have _IfcTableColumn_ instances that define the name, description and units for each column. The rows of information are stored as a list of _IfcTableRow_ objects.

Limitation: For backwards compatibility, the rows of an _IfcTable_ object are constrained to have the same number of cells. The first row of the table provides the number of cells. All other rows are forced to include the same number of cells. This is enforced by the WR2.

Figure 1 illustrates table use.

!(../../../../../../figures/ifctable_image1.gif "Figure 1 &mdash; Table use")

Figure 2 depicts how tables were structured prior to IFC4.

!(../../../../../../figures/ifctable_image2.gif "Figure 2 &mdash; Table use alternative")

> HISTORY&nbsp; New entity in IFC1.5.

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Columns attribute added.
