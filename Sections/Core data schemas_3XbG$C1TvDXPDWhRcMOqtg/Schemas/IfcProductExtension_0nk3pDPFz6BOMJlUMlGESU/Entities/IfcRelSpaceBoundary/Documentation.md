The space boundary (_IfcRelSpaceBoundary_) defines the physical or virtual delimiter of a space as its relationship to the surrounding elements.

* In the case of physical space boundary, the placement and shape of the boundary may be given, and the building element, providing the boundary, is referenced, 
* In the case of virtual space boundary, the placement and shape of the boundary may be given, but no building element is referenced. 

The exact definition of how space boundaries are broken down depends on the view, more detailed conventions on how space boundaries are decomposed can only be given at the domain or application type level.

> <font size="-1">EXAMPLE: In an architectural or FM
        related view, a space boundary is defined from the inside
        of the space and does not take the providing building
        element into account. A plane area (even if the building
        element changes) is still seen as a single space
        boundary. In an HVAC related view, the decomposition of
        the space boundary depends on the material of the
        providing building element and the adjacent spaces
        behind.</font>
> 


> <font color="#0000FF" size="-1">HISTORY: New entity in IFC
      Release 1.5, the entity has been modified in IFC Release 2x
      .</font>

> <font color="#FF0000" size="-1">IFC2x PLATFORM CHANGE: The
      data type of the attribute<i>RelatedBuildingElement</i> has
      been changed from <i>IfcBuildingElement</i> to its
      supertype <i>IfcElement</i> with upward compatibility for
      file based exchange. The data type of the attribute
      <i>ConnectionGeometry</i> has been changed from
      <i>IfcConnectionSurfaceGeometry</i> to its supertype
      <i>IfcConnectionGeometry</i> with upward compatibility for
      file based exchange.</font>

The _IfcRelSpaceBoundary_ is defined as an objectified relationship that handles the element to space relationship by objectifying the relationship between an element and the space it bounds. It is given as a one-to-one relationship, but allows each building element to define many such relationship and each space to be defined by many such relationships.

> <font color="#FF0000" size="-1">Note: With the upward
      compatible platform extension the
      <i>IfcRelSpaceBoundary</i> can now also be given to an
      <i>IfcOpeningElement</i>.</font>

****Use Definitions****

If the _IfcRelSpaceBoundary_ is used to express a virtual boundary, the attribute _PhysicalOrVirtualBoundary_ has to be set to VIRTUAL. If this virtual boundary is between two spaces, and the correct location is of interest, the attribute _RelatedBuildingElement_ shall point to an instance of _IfcVirtualElement_, and the attribute _ConnectionGeometry_ is required to be inserted.

> <font size="-1">NOTE: The connection geometry, either by a
      2D curve or a 3D surface, is used to describe the portion
      of the "virtual wall" that separates the two spaces. All
      instances of <i>IfcRelSpaceBoundary</i> given at the
      adjacent spaces share the same instance of
      <i>IfcVirtualElement</i>. Each instance of
      <i>IfcRelSpaceBoundary</i> provides in addition the
      <i>ConnectionGeometry</i> given within the local placement
      of each space.</font>

> <font size="-1" color="#FF0000">NOTE:
      <i>IfcVirtualElement</i> has been introduced in IFC2x2
      Addendum 1 to facilitate virtual space boundaries.</font>

If the _IfcRelSpaceBoundary_ is used to express a physical boundary between two spaces, the attribute _PhysicalOrVirtualBoundary_ has to be set to PHYSICAL. The attribute _RelatedBuildingElement_ has to be given and points to the element providing the space boundary. The attribute _ConnectionGeometry_ may be inserted, in this case it describes the physical space boundary geometrically, or it may be omitted, in that case it describes a physical space boundary logically.

****Geometry Use Definitions****:

The _IfcRelSpaceBoundary_ may have geometry attached. If geometry is not attached, the relationship between space and building element is handled only on a logical level. If geometry is attached, it is given within the local coordinate systems of the space and (if given in addition) of the building element.

> <font size="-1">NOTE: The attributes
        <i>CurveOnRelatingElement</i> at
        <i>IfcConnectionCurveGeometry</i> or
        <i>SurfaceOnRelatingElement</i> at
        <i>IfcConnectionSurfaceGeometry</i> provide the geometry
        within the local coordinate system of the
        <i>IfcSpace</i>, whereas the attributes
        <i>CurveOnRelatedElement</i> at
        <i>IfcConnectionCurveGeometry</i> or
        <i>SurfaceOnRelatedElement</i> at
        <i>IfcConnectionSurfaceGeometry</i> provide the geometry
        within the local coordinate system of the subtype of
        <i>IfcElement</i>.</font>
> 


The connection geometry, when given, can be given as a curve (for 2D representations of space boundaries) or as a surface (for 3D representations of space boundaries).

> <font color="#FF0000" size="-1">Note: With the upward
      compatible platform extension the <i>ConnectionGeometry</i>
      can now also be given by a 2D curve.</font>

The geometric representation (through the _ConnectionGeometry_ attribute) is defined using either 2D curve geometry or extruded surfaces for space boundaries which bounds prismatic spaces.

The following constraints apply to the 2D curve representation:

* Curve: _IfcPolyline_, _IfcTrimmedCurve_ or _IfcCompositeCurve_ 

The following constraints apply to the surface representation:

*  **Surface**: _IfcSurfaceOfLinearExtrusion_ 
*  **Profile**: _IfcArbitraryOpenProfileDef_ 
*  **Extrusion**: The extrusion direction shall be vertically, i.e., along the positive Z Axis of the co-ordinate system of the containing spatial structure element.