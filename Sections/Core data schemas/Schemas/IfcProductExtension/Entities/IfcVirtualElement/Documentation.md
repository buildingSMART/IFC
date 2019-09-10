A special element used to provide imaginary boundaries, such as between two adjacent, but not separated, spaces. Virtual elements are usually not displayed and does not have quantities and other measures. Therefore _IfcVirtualElement_ does not have material information and quantities attached.

> <small>NOTE The main purpose of <i>IfcVirtualElement</i> is
      the provision of a virtual space boundary. The
      <i>IfcVirtualElement</i> provides the 2D curve or 3D
      surface representation of the virtual space connection and
      is referenced by two instances of
      <i>IfcRelSpaceBoundary</i>, each pointing to one of the two
      adjacent <i>IfcSpaces</i>.</small>

> <small><font color="#0000FF">HISTORY New entity in IFC
      Release 2x2 Addendum.</font></small>

> <small><font color="#FF0000">IFC2x2 ADDENDUM CHANGE: The
      entity <i>IfcVirtualElement</i> has been added. Upward
      compatibility for file based exchange is
      guaranteed.</font></small>

****Geometry Use Definitions****

The geometric representation of any _IfcVirtualElement_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

**Local Placement**

The local placement for _IfcVirtualElement_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_ that is used in the _ContainedInStructure_ inverse attribute or to a referenced spatial structure element at a higher level. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

**_Geometric Representations_**

Currently, the use of 'FootPrint' and 'Surface' representation is supported.

**Two-dimensional Representation using foot print
      representation**

The 2D geometric representation of _IfcVirtualElement_ is defined using the 'FootPrint' or 'Surface' representation. The following attribute values should be inserted

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'FootPrint'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'Curve2D' or 'GeometricCurveSet' . 

The following constraints apply to the 2D curve representation:

* Curve: _IfcPolyline_, _IfcTrimmedCurve_ or _IfcCompositeCurve_ 

**Three-dimensional Representation using surface model
      representation**

The 3D geometric representation of _IfcVirtualElement_ is defined using the 'SurfaceModel' geometry. The following attribute values should be inserted

*  _IfcShapeRepresentation.RepresentationIdentifier_ = 'Surface'. 
*  _IfcShapeRepresentation.RepresentationType_ = 'GeometricSet . 

The following constraints apply to the 3D surface representation:

*  **Surface**: _IfcSurfaceOfLinearExtrusion_ 
*  **Profile**: _IfcArbitraryOpenProfileDef_ 
*  **Extrusion**: The extrusion direction shall be vertically, i.e., along the positive Z Axis of the co-ordinate system of the containing spatial structure element.