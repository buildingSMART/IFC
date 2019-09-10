The schema _IfcGeometricConstraintResource_ defines the resources used to determine the placement of the shape representation of a product within the geometric representation context of a project. It also contains resource definitions to be assigned to product connectivity definitions to determine the connection geometry constraints between those products.

The primary application of this resource is to:

* determine the object placement used for the shape representation of the object
* determine the constraints applied to the connectivity between two shapes of objects

### Placement
The placement of an product's shape is given by the _IfcObjectPlacement_, referred to by the _IfcProduct.ObjectPlacement_. The object placement defines the object coordinate system in which all shape representations of that product are defined. It is given either as

* absolute placement
* relative placement
* placement relative to a grid

The absolute placement is specified by using _IfcLocalPlacement_ and omitting the _PlacementRelTo_ attribute. The relative placement is specified by using _IfcLocalPlacement_ and pointing the _PlacementRelTo_ attribute to an _IfcObjectPlacement_ used in another _IfcProduct_ instance.

A placement relative to a grid is given by _IfcGridPlacement_ pointing to one (or two) virtual intersections of _IfcGridAxis_. If two virtual intersections are references, than the second virtual intersections specifies the orientation of the object placement.

### Connection geometry
The connection geometry constrains the connectivity between the shapes of two products. The constraint can be defined by geometric representation items:

* point
* curve
* surface

or by topological representation items with associated geometry:

* vertex point
* edge curve
* face surface

As a special type of point connection includes the provision to express an eccentricity, i.e. a physical distance between the two points involved in the connection.