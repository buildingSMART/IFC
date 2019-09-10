An annotation is a graphical representation within the geometric (and spatial) context of a project, that adds a note or meaning to the objects which constitutes the project model. Annotations include additional points, curves, text, dimensioning, hatching and other forms of graphical notes. It also include symbolic representations of additional model components, not representing products or spatial structures, such as survey points, contour lines or similar.

> NOTE&nbsp; Additional presentation information (often 2D) such as tag number or hatching, that is directly related to a particular product representation is included within the _IfcProductDefinitionShape_ having various _IfcShapeRepresentation_'s of the _IfcElement_ (and its subtypes). Only those presentation information, that cannot be directly related to a single product, have to be wrapped within the _IfcAnnotation_.

If available, the annotation should be related to the spatial context of the project, by containing the annotation within the appropriate level of the building structure (site, building, storey, or space). This is handled by the _IfcRelContainedInSpatialStructure_ relationship.

> HISTORY&nbsp; New entity in IFC2x2.

{ .use-head}
Attribute use definition

The _IfcAnnotation_ can provide specific 0D, 1D, and 2D geometric items as representation of the annotation, offering annotation point, curves, and surfaces. The following values shall be used for the _ObjectType_.

*  **'Annotation point'** is an annotation provided by a point that has additional semantic. The inherited attribute _ObjectType_ should be used to capture the type of point annotation, some predefined values are: 
    * '**SurveyPoint**: A single survey point represented by a Cartesian point. A property set may add the conditions (method, accurracy, etc. to the survey point). 
    * '**SurveyArea**': A set of survey points represented by Cartesian point. These coordinates are determined relative to the coordinates of a reference point, which acts as the datum for the survey. Properties attached apply equally to all points. The difference in elevation of the survey points enables terrain to be determined. 
*  **'Annotation curve'** is an annotation provided by a curve that has additional semantic. The inherited attribute _ObjectType_ should be used to capture the type of curve annotation, some predefined values are: 
    * '**ContourLine**': A line of constant elevation typically used on geographic maps where the spacing of lines at constant intervals of elevation may be used as an indication of slope. 
    * '**IsoBar**': A line of constant pressure typically used on weather maps or to show pressure gradient in spaces, chambers or externally. 
    * '**IsoLux**': A line of constant illumination typically used to show the distribution of illumination levels and/or daylighting in a space or externally. 
    * '**IsoTherm**': A line of constant temperature typically used to show the distribution and effect of heating or cooling within a space or to show temperature distribution on a geographic map. 
*  **'Annotation surface'** is an annotation provided by a surface that has additional semantic. The inherited attribute _ObjectType_ should be used to capture the type of surface annotation, some predefined values are: 
    * '**SurveyArea**': A surface patch based on survey points. 

___
## Common Use Definitions
The following concepts are inherited at supertypes:

* _IfcRoot_: [Identity](../../templates/identity.htm), [Revision Control](../../templates/revision-control.htm)

[![Image](../../../img/diagram.png)&nbsp;Instance diagram](../../../annex/annex-d/common-use-definitions/ifcannotation.htm)

{ .use-head}
Property Sets for Objects

The [Property Sets for Objects](../../templates/property-sets-for-objects.htm) concept applies to this entity as shown in Table 1.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>PredefinedType</b></th><th><b>Name</b></th></tr>
<tr><td>ContourLine</td><td><a href="../../psd/ifcproductextension/Pset_AnnotationContourLine.xml">Pset_AnnotationContourLine</a></td></tr>
<tr><td>LineOfSight</td><td><a href="../../psd/ifcproductextension/Pset_AnnotationLineOfSight.xml">Pset_AnnotationLineOfSight</a></td></tr>
<tr><td>SurveyArea</td><td><a href="../../psd/ifcproductextension/Pset_AnnotationSurveyArea.xml">Pset_AnnotationSurveyArea</a></td></tr>
<tr><td>Sound</td><td><a href="../../psd/ifcsharedbldgserviceelements/Pset_SoundAttenuation.xml">Pset_SoundAttenuation</a></td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 1 &mdash; IfcAnnotation Property Sets for Objects</p></td></tr></table>

  
  
{ .use-head}
Annotation 2D Geometry

The [Annotation 2D Geometry](../../templates/annotation-2d-geometry.htm) concept applies to this entity as shown in Table 2.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>Annotation</td><td>Annotation2D</td><td><a href="../../ifcgeometricmodelresource/lexical/ifcgeometriccurveset.htm">IfcGeometricCurveSet</a></td><td>Any point or curve</td></tr>
<tr><td>Annotation</td><td>Annotation2D</td><td><a href="../../ifcpresentationdefinitionresource/lexical/ifcannotationfillarea.htm">IfcAnnotationFillArea</a></td><td>Area for hatching</td></tr>
<tr><td>Annotation</td><td>Annotation2D</td><td><a href="../../ifcpresentationdefinitionresource/lexical/ifctextliteral.htm">IfcTextLiteral</a></td><td>Text literal for applying text</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 2 &mdash; IfcAnnotation Annotation 2D Geometry</p></td></tr></table>

  
  
{ .use-head}
Annotation 3D Geometry

The [Annotation 3D Geometry](../../templates/annotation-3d-geometry.htm) concept applies to this entity as shown in Table 3.

<table>
<tr><td>
<table class="gridtable">
<tr><th><b>Identifier</b></th><th><b>Type</b></th><th><b>Items</b></th><th><b>Description</b></th></tr>
<tr><td>Annotation</td><td>GeometricSet</td><td><a href="../../ifcgeometricmodelresource/lexical/ifcgeometricset.htm">IfcGeometricSet</a></td><td>Any point, curve or surface representing the annotation.</td></tr>
</table>
</td></tr>
<tr><td><p class="table">Table 3 &mdash; IfcAnnotation Annotation 3D Geometry</p></td></tr></table>
