**Definition from ISO/CD 10303-42:1992**: This function produces a three dimensional direction which is, with fully defined input, the projection of arg onto the plane normal to the z-axis. With arg defaulted the result is the projection of (1.0,0.0,0.0) onto this plane except that if z-axis = (1.0,0.0,0.0) then (0.0,1.0,0.0) is used as initial value of arg. A violation occurs if arg is in the same direction as the input z-axis.

> <small><font color="#0000ff">NOTE
&nbsp;Corresponding STEP function: first_proj_axis. Please refer
to ISO/IS
10303-42:1994, p.102 for the final definition of the formal
standard.&nbsp; <br>
  <br>
HISTORY&nbsp; New function in IFC Release 1.5 </font></small>