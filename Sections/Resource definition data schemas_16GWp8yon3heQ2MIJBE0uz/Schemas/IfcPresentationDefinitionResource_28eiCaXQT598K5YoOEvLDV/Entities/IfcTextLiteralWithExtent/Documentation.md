The text literal with extent is a text literal with the additional explicit information of the planar extent. An alignment attribute defines how the text box is aligned to the placement and how it may expand if additional lines of text need to be added.

Figure 1 shows the use of planar extent and box alignment to position the text string

!["IfcTextLiteralWithExtent_Fig1.png 8,1 KB"](../../../figures/ifctextliteralwithextent_fig1.png "Figure 1 &mdash; Text literal with extent and alignment")

The planar extent defines the box model within which the text is placed. Padding maybe defined in the text style that offsets the text from the box to its inside.

> NOTE&nbsp; Entity adapted from **text_literal_with_extent** defined in ISO10303-46

> HISTORY&nbsp; New entity in IFC2x2.

{ .change-ifc2x3}
> IFC2x3 CHANGE &nbsp;The _IfcTextLiteralWithExtent_ has been changed by adding _BoxAlignment_.