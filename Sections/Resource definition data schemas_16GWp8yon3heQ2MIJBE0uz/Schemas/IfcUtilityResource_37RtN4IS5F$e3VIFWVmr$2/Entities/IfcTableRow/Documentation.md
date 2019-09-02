The information content of each row within the table (other than the heading row). A table contains a number of rows which record information concerning the instance of the type of information recorded within the table.

Limitation: Within this release of IFC all _IfcTableRow_ objects referenced by an _IfcTable_ shall have the same number of Row Cells. The actual number of Cells shall be taken from the number of cells of the first _IfcTableRow_ for that table. The number of Cells is calculated by the derived attribute _NumberOfCellsInRow_ in the associated _IfcTable_.

![Image](figures/IfcTableRow_Image1.gif)

> <font color="#0000FF" size="-1"> HISTORY: New entity in IFC R1.5.<br>
		  </font>
>