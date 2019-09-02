An _IfcCartesianTransformationOperator_ defines an abstract supertype of different kinds of geometric transformations.

{ .extDef}
> NOTE&nbsp; Definition according to ISO/CD 10303-42:1992  
> A Cartesian transformation operator defines a geometric transformation composed of translation, rotation, mirroring and uniform scaling. The list of normalized vectors u defines the columns of an orthogonal matrix T. These vectors are computed, by the base axis function, from the direction attributes axis1, axis2 and, in Cartesian transformation operator 3d, axis3. If **|T|= -1**, the transformation includes mirroring. The local origin point **A**, the scale value **_S_** and the matrix **T** together define a transformation.  
>   
> The transformation for a point with position vector P is defined by 
>> P -&gt; A + _S_TP
> The transformation for a direction d is defined by
> 
>> d -&gt; Td
> The transformation for a vector with orientation d and magnitude k is defined by
> 
>> d -&gt; Td, and  
>> _k -&gt; Sk_
> For those entities whose attributes include an axis2 placement, the transformation is applied, after the derivation, to the derived attributes p defining the placement coordinate directions. For a transformed surface, the direction of the surface normal at any point is obtained by transforming the normal, at the corresponding point, to the original surface. For geometric entities with attributes (such as the radius of a circle) which have the dimensionality of length, the values will be multiplied by _S_.
> 
> For curves on surface the p curve.reference to curve will be unaffected by any transformation. The Cartesian transformation operator shall only be applied to geometry defined in a consistent system of units with the same units on each axis. With all optional attributes omitted, the transformation defaults to the identity transformation. The Cartesian transformation operator shall only be instantiated as one of its subtypes.
> 


> NOTE&nbsp; Entity adapted from **cartesian_transformation_operator** defined in ISO10303-42.

> HISTORY&nbsp; New entity in IFC2x.