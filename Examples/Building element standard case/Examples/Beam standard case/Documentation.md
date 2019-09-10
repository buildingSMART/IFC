{ .std}
The _IfcBeamStandardCase_ is a standard case element to exchange parametric definitions of the beam shape.

{ .std}
The example includes the local placement, the body shape representation, the material profile set assignment, the beam occurrence and beam type definitions. The focus points are the use of cardinal points to align the beam profile to the axis, the use of parametric profile definitions and the assignment of material information to the profile.

{ .std}
*  [Beam standard case with hyperlinks](ifc/standard_case_element_beam.ifc.htm){ .listing-link target="info"} 
*  [Beam standard case source file](ifc/standard_case_element_beam.ifc){ .listing-link target="info"} 

&nbsp;

<table summary="beam example">
        <tr>
          <td>
            <img src="fig/standard_case_element_beam-1.png" width="610" height="210" alt="standard_case_element_beam-2.png 44,2 KB">
          </td>
          <td style=" vertical-align:bottom;">
            <p>
              The example in Figure E11 declares two parametric beam types, one with an I-Shape
              profile and the other with a T-Shape profile. Each type has nine occurrences, using various cardinal
              points to align the profiles.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p class="figure">
              Figure E11 &mdash; Beam occurrences
            </p>
            <p>
              &nbsp;
            </p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
        <tr>
          <td>
            <img src="fig/standard_case_element_beam-2.png" width="308" height="258" alt="standard_case_element_beam-2.png 2,6 KB">
          </td>
          <td style=" vertical-align:bottom;">
            <p>
              The beam 'A-9' in Figure E12 is an occurrence of the 'IPE220' type having an
              I-Shape profile, placed along an axis using the upper-right cardinal point.
            </p>
            <p>
              The cardinal point of the beam 'A-9' is set to the upper-right, indicating that the 'Body' representation
              should be generated with the upper-right of the profile aligned along the curve of the 'Axis
              representation.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p class="figure">
              Figure E12 &mdash; Beam profile and cardinal point usage
            </p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
      </table>

&nbsp;

<table summary="beam example" cellpadding="2">
        <tr>
          <td>
            <img src="fig/standard_case_element_beam-3.png" width="610" height="226" alt="standard_case_element_beam-3.png 18,1 KB">
          </td>
          <td style=" vertical-align:bottom;">
            <p>
              The 'IPE220' beam type in Figure E13 is represented by <i>IfcBeamType</i>. As a
              parametric definition, this beam type does not have any geometric representation, rather it has a
              material profile set association indicating a cross-section which may be applied to paths defined at
              occurrences.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p class="figure">
              Figure E13 &mdash; Beam type graph
            </p>
            <p>
              &nbsp;
            </p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
      </table>

<table summary="beam example" cellpadding="2">
        <tr>
          <td>
            <img src="fig/standard_case_element_beam-4.png" width="610" height="372" alt="standard_case_element_beam-2.png 21,2 KB">
          </td>
          <td style=" vertical-align:bottom;">
            <p>
              Each beam occurrence as in Figure E14 is represented by
              <i>IfcBeamStandardCase</i>. The <i>IfcMaterialProfileSetUsage</i> entity indicates the alignment of the
              material profile set according to cardinal point. The <i>IfcMaterialProfileSet</i> indicates a single
              material profile. The <i>IfcMaterialProfile</i> indicates an I-Shape cross-section of steel. The
              <i>IfcIShapeProfileDef</i> indicates shape parameters of the I-Shape profile. The <i>IfcMaterial</i>
              indicates the steel material, which could be further elaborated with structural properties, surface
              styles, and fill area styles.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p class="figure">
              Figure E14 &mdash; Beam occurrence graph
            </p>
          </td>
          <td>
            &nbsp;
          </td>
        </tr>
      </table>