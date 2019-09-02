**Definition
from IAI**: The _IfcGeometricRepresentationSubContext_ defines the context that applies to several shape representations of a product being a sub context, sharing the _WorldCoordinateSystem_, _CoordinateSpaceDimension_, _Precision_ and _TrueNorth_ attributes with the parent _IfcGeometricRepresentationContext_.

The _IfcGeometricRepresentationSubContext_ is used to define semantically distinguished representation types for different information content, dependent on the representation view and the target scale. It can be used to control the level of detail of the shape representation that is most applicable to this geometric representation context. addition the sub context is used to control the later appearance of the _IfcShapeRepresentation_within a plot view.

> <small>NOTE&nbsp;
If the <i>IfcShapeRepresentation</i>
using this sub context has<i>
IfcStyledItem</i>'s assigned to the <i>Items</i>,
the presentation style information (e.g. <i>IfcCurveStyle</i>,
  <i>IfcTextStyle</i>)
associated with the <i>IfcStyledItem</i>
is given in target
plot dimensions. E.g. a line thickness (<i>IfcCurveStyle.CurveWidth</i>)
is given by a thickness measure relating to the thickness for a plot
within the (range of) target scale.</small>
> 


Each _IfcProduct_ can then have several instances of subtypes of _IfcRepresentation_, each being assigned to a different geometric representation context (_IfcGeometricRepresentationContext_ or _IfcGeometricRepresentationSubContext_). The application can then choose the most appropriate representation for showing the geometric shape of the product, depending on the target view and scale.

> <small>NOTE
The provision of a model view
(<i>IfcGeometricRepresentationContext.ContextType</i>
= 'Model') is mandatory. Instances of <i>IfcGeometricRepresentationSubContext</i>
relate to it as its <i>ParentContext</i>.</small>
> 


> <small>EXAMPLE&nbsp;
Instances
of <i>IfcGeometricRepresentationSubContext</i>
can be used to handle the multi-view blocks or macros,
which are used
in CAD programs to store several scale and/or view dependent geometric
representations of the same object.</small>
> 


> <font color="#0000ff" size="-1">HISTORY New entity
in Release IFC 2x Edition 2.</font>
>