The _IfcProduct_ is an abstract representation of any object that relates to a geometric or spatial context. Subtypes of _IfcProduct_ usually hold a shape representation and an object placement within the project structure.

This includes manufactured, supplied or created objects (referred to as elements) for incorporation into an AEC/FM project. This also includes objects that are created indirectly by other products, as spaces are defined by bounding elements. Products can be designated for permanent use or temporary use, an example for the latter is formwork. Products are defined by their properties and representations.

In addition to physical products (covered by the subtype _IfcElement_) and spatial items (covered by the subtype _IfcSpatialElement_) the _IfcProduct_ also includes non-physical items, that relate to a geometric or spatial contexts, such as grid, port, annotation, structural actions, etc.

The inherited _ObjectType_ attribute can be used to designate a particular type of the product instance. If subtypes of _IfcProduct_ have a _PredefinedType_ defined, the _ObjectType_ is used to provide the user defined, particular type of the product instance, if the _PredefinedType_ is set to <small>USERDEFINED</small>.

> HISTORY&nbsp; New entity in IFC1.0

{ .use-head}
Generic relationship use definition

On a generic level products can be assigned to processes, controls, resources, project by using the relationship objects that refer to the corresponding object:

<ul>
<li><b>Having a control applied</b>: assigned using
<em>IfcRelAssignsToControl</em> linking the <em>IfcProduct</em> to an
<em>IfcControl</em>
<ul>
<li style="list-style-type:none"><small>An example of this
relationship is the assignment of a performance history to a
distribution element.</small></li>
</ul>
</li>
<li><b>Being assigned to a process</b>: assigned using
<em>IfcRelAssignsToProcess</em> linking the <em>IfcProduct</em> to an
<em>IfcProcess</em>
<ul>
<li style="list-style-type:none"><small>An example of this
relationship is the assignment of products like wall, slab,
column to a contruction task for construction
planning.</small></li>
</ul>
</li>
<li><b>Being assigned to a resource</b>: assigned using
<em>IfcRelAssignsToResource</em> linking the <em>IfcProduct</em> to
an <em>IfcResource</em>
<ul>
<li style="list-style-type:none"><small>An example of this
relationship is the assignment of products to a construction
resource that consumes the product.</small></li>
</ul>
</li>
</ul>
{ .use-head}
Generic type use definition

Any instance of _IfcProduct_ defines a particular occurrence of a product, the common type information, that relates to many similar (or identical) occurrences of _IfcProduct_, is handled by the _IfcTypeProduct_ (and its subtypes), assigned to one or many occurrences of _IfcProduct_ by using the objectified relationship _IfcRelDefinesByType_. The _IfcTypeProduct_ may provide, in addition to common properties, also a common geometric representation for all occurrences.

> NOTE&nbsp; See _IfcTypeProduct_ for how to use a common geometric representation and _IfcRelDefinesByType_ for using and overriding common properties.

{ .use-head}
Generic representation use definition

An _IfcProduct_ occurs at a specific location in space if it has a geometric representation assigned. It can be placed relatively to other products, but ultimately relative to the world coordinate system defined for this project. The _ObjectPlacement_ attribute establishes the coordinate system in which all points and directions used by the geometric representation items under <small>Representation</small> are founded. The placement can either be:

* **a relative placement**: by _IfcLocalPlacement_ with _PlacementRelTo_ pointing to a parent placement
* **an absolute placement**: by _IfcLocalPlacement_ with _PlacementRelTo_ being NIL
* **a placement relative to a grid**: by _IfcGridPlacement_

The _Representation_ is provided by an _IfcProductDefinitionShape_ being either a geometric shape representation, or a topology representation (with or without underlying geometry of the topological items).