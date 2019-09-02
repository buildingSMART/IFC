An annotation is a graphical representation within the geometric (and spatial) context of a project, that adds a note or meaning to the objects which constitutes the project model. Annotations include additional line drawings, text, dimensioning, hatching and other forms of graphical notes.

> <small>NOTE Additional presentation information (often
        2D) such as tag number, hatching, etc., that is directly
        related to a particular product representation is
        included within the <i>IfcProductDefinitionShape</i>
        having various <i>IfcShapeRepresentation</i>'s of the
        <i>IfcElement</i> (and its subtypes). Only those
        presentation information, that cannot be directly related
        to a single product, have to be wrapped within the
        <i>IfcAnnotation</i>.</small>
> 


If available, the annotation should be related to the spatial context of the project, by containing the annotation within the appropriate level of the building structure (site, building, storey, or space). This is handled by the _IfcRelContainedInSpatialStructure_ relationship.

> <font color="#0000FF" size="-1">HISTORY: New entity in
        Release IFC2x Edition 2.</font>
> 


****Geometry Use Definitions****

The geometric representation of any _IfcAnnotation_ is given by the _IfcProductDefinitionShape_ and _IfcLocalPlacement_ allowing multiple geometric representations.

**Local Placement**

The local placement for any _IfcAnnotation_ is defined in its supertype _IfcProduct_. It is defined by the _IfcLocalPlacement_, which defines the local coordinate system that is referenced by all geometric representations.

* The _PlacementRelTo_ relationship of _IfcLocalPlacement_ shall point (if given) to the local placement of the same _IfcSpatialStructureElement_, which is used in the _ContainedInStructure_ inverse attribute, or to a spatial structure element at a higher level, referenced by that. 
* If the relative placement is not used, the absolute placement is defined within the world coordinate system. 

_**Geometric Representations**_

The standard representation of _IfcAnnotation_ is defined using 'GeometricCurveSet' or, when including surfaces, the 'GeometricSet' geometry. Styled items adding the style information assigned to the geometric representation items are grouped together with the geometric representation items within the set of _Items_ at _IfcShapeRepresentation_.