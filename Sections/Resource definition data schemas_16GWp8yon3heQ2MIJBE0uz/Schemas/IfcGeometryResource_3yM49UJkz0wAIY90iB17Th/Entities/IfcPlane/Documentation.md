**Definition from ISO/CD 10303-42:1992**: A plane is an unbounded surface with a constant normal. A plane is defined by a point on the plane and the normal direction to the plane. The data is to be interpreted as follows:

> 
>> <pre>C = SELF\IfcElementarySurface.Position.Location
x = SELF\IfcElementarySurface.Position.P[1]
y = SELF\IfcElementarySurface.Position.P[2]
z = SELF\IfcElementarySurface.Position.P[3] =&gt; normal to plane</pre>


> 
and the surface is parameterized as:

> 
>> ![Image](figures/IfcPlane-Math1.gif.gif)
>>


> 
where the parametric range is -&infin; &lt; _u,v_ &lt; &infin; .

In the above parameterization the length unit for the unit vectors **x** and **y** is derived from the context of the plane.

> <font size="-1" color="#0000FF">NOTE Corresponding STEP entity: plane.
		  Please refer to ISO/IS 10303-42:1994, p.69 for the final definition of the
		  formal standard. </font>
> 
> <font color="#0000FF" size="-1">HISTORY New class in IFC Release 1.5
		  </font>
>