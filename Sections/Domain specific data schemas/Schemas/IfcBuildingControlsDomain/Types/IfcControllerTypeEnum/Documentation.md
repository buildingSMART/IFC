The _IfcControllerTypeEnum_ defines the range of different types of controller that can be specified.

> <font color="#0000FF" size="-1"> HISTORY: New type in IFC R2.0</font>
> 


**Enumeration**

<table border="1"> 
		<tr> 
		  <td><i>Value</i></td> 
		  <td><i>Definition</i></td> 
		  <td><i>Pset</i></td> 
		</tr> 
		<tr> 
		  <td>FLOATING</td> 
		  <td>Output increases or decreases at a constant or accelerating
			 rate</td> 
		  <td>NO</td> 
		</tr> 
		<tr> 
		  <td>PROPORTIONAL</td> 
		  <td>Output is proportional to the control error</td> 
		  <td>NO</td> 
		</tr> 
		<tr> 
		  <td>PROPORTIONALINTEGRAL</td> 
		  <td>Part of the output is proportional to the control error and part is
			 proportional to the time integral of the control error</td> 
		  <td>NO</td> 
		</tr> 
		<tr> 
		  <td>PROPORTIONALINTEGRALDERIVATIVE</td> 
		  <td>part of the output is proportional to the control error, part is
			 proportional to the time integral of the control error and part is proportional
			 to the time derivative of the control error</td> 
		  <td>NO</td> 
		</tr> 
		<tr> 
		  <td>TIMEDTWOPOSITION</td> 
		  <td>Output changes state for a time interval proportional to the
			 deviation from setpoint</td> 
		  <td>NO</td> 
		</tr> 
		<tr> 
		  <td>TWOPOSITION</td> 
		  <td>Binary output, can be either on or off</td> 
		  <td>NO</td> 
		</tr> 
		<tr> 
		  <td>USERDEFINED</td> 
		  <td></td> 
		  <td></td> 
		</tr> 
		<tr> 
		  <td>NOTDEFINED</td> 
		  <td></td> 
		  <td></td> 
		</tr> 
	 </table>
