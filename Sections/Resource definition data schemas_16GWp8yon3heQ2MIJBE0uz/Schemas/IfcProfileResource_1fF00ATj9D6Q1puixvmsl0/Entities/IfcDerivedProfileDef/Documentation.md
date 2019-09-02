**Definition
from IAI**: The _IfcDerivedProfileDef_ defines the profile by transformation from the parent profile. The transformation is given by a two dimensional transformation operator. Transformation includes translation, rotation, mirror and scaling. The latter can be uniform or non uniform. The derived profiles may be used to define swept surfaces, swept area solids or sectioned spines.

The transformation effects the position, rotation, mirroring or scale of the profile at the underlying coordinate system, i.e. the coordinate system defined by the swept surface or swept area solid that uses the profile definition. It is the xy plane of either:

* _IfcSweptSurface.Position_
* _IfcSweptAreaSolid.Position_


or in case of sectioned spines the xy plane of each list member of _IfcSectionedSpine.CrossSectionPositions_.
The position and potential rotation of the _ParentProfile_
within
the underlying coordinate system is taken into consideration before
applying the Cartesian transformation operator.
> <font color="#0000ff" size="-1">HISTORY: New entity
in IFC Release 2x.</font>

**Illustration**:

<table border="1" cellpadding="2" cellspacing="2">
  <tbody>
    <tr>
      <td align="left" valign="top" width="405"><a href="drawings/IfcDerivedProfileDef-Layout1.dwf"><img src="figures/IfcDerivedProfileDef-Layout1.gif" alt="uniform" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">
      <p><u>Parameter</u>
      <br>
The <i>IfcDerivedProfileDef</i>
is defined using the <i>IfcCartesianTransformationOperator2D</i>
(CTO), which is applied to the parent profile definition. <br>
      </p>
      <p><u>Example</u><br>
The example shows an uniform scaling and a transformation
of an <i>IfcRectangleProfileDef</i>
to match the lower-left cardinal point. The attributes of the CTO are:<br>
      </p>
      <blockquote><tt>Axis1
= NIL (defaults
to 1.,0.)<br>
Axis2
= NIL (defaults to 0.,1.)<br>
LocalOrigin =
IfcCartesianPoint(&lt;1/2 XDim&gt;,&lt;1/2 YDim&gt;)<br>
Scale = 2.<br>
        </tt></blockquote>
      <font size="-1">Note:
The <i>ParentProfile</i>
has a <i>Position</i>
= <i>IfcCartesianPoint</i>(&lt;1/2
XDim&gt;,&lt;1/2 YDim&gt;) already.</font><br>
      <blockquote><tt></tt></blockquote>
      </td>
    </tr>
    <tr>
      <td align="left" valign="top" width="405"><a href="drawings/IfcDerivedProfileDef-Layout2.dwf"><img src="figures/IfcDerivedProfileDef-Layout2.gif" alt="non uniform" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">
      <p><u>Parameter</u>
      <br>
The <i>IfcDerivedProfileDef</i>
is defined using
non uniform transformationsby applying the <i>IfcCartesianTransformationOperator2DnonUniform</i>
as a subtype of the 2D CTO.</p>
      <p><u>Example</u><br>
The example shows a non-uniform scaling and a translation of an <i>IfcRectangleProfileDef</i>
to match the lower-left cardinal point. The attributes of the CTO are:</p>
      <blockquote> <tt>Axis1
= NIL (defaults to 1.,0.)<br>
Axis2 = NIL (defaults to 0.,1.)<br>
LocalOrigin = IfcCartesianPoint(0.,&lt;1/2 YDim)<br>
Scale&nbsp; = 1.<br>
Scale2 = 2.<br>
        </tt></blockquote>
      <font size="-1">Note:
The <i>ParentProfile</i>
has a <i>Position</i>
= <i>IfcCartesianPoint</i>(&lt;1/2
XDim&gt;,&lt;1/2 YDim&gt;) already.</font>
      </td>
    </tr>
    <tr>
      <td><a href="drawings/IfcDerivedProfileDef-Layout3.dwf"><img alt="mirroring" src="figures/IfcDerivedProfileDef-Layout3.gif" border="0" height="300" width="400"></a></td>
      <td align="left" valign="top">
      <p><u>Parameter</u>
      <br>
The <i>IfcDerivedProfileDef</i>
is defined using mirroring by applying the <i>IfcCartesianTransformationOperator2D</i>
(CTO) to the parent profile.</p>
      <p><u>Example</u><br>
The example shows a mirroring of an <i>IfcLShapeProfileDef</i>
to match the centre cardinal point. The attributes of the CTO are:</p>
      <blockquote><tt>Axis1
= </tt><tt>(0.,-1.)</tt><tt></tt><br>
        <tt>Axis2 = </tt><tt>NIL
(defaults to 1.,0.)</tt><br>
        <tt>LocalOrigin =
IfcCartesianPoint(0.,0.)</tt><br>
        <tt>Scale = NIL (defaults
to 1.)<br>
        </tt></blockquote>
      <font size="-1">Note:
The <i>ParentProfile</i>
has a <i>Position</i>
= <i>IfcCartesianPoint</i>(0.,0.).</font></td>
    </tr>
    <tr>
      <td colspan="2" rowspan="1" align="left" valign="top" width="405"><font size="-1">Note:
The following color map applies:<br>
      </font>
      <ul>
        <li><font size="-1">black coordinate axes show the
underlying coordinate system of the swept surface, swept area solid, or
sectioned spine</font></li>
        <li><font size="-1"><font color="#ff0000">red coordinate axes</font>
show the position coordinate system of the parent profile</font></li>
        <li><font size="-1"><font color="#993300">brown coordinate axes</font>
show the position coordinate system of the derived profi<br>
          </font></li>
      </ul>
      </td>
    </tr>
  </tbody>
</table>

Table: Derivation of derived profile definition