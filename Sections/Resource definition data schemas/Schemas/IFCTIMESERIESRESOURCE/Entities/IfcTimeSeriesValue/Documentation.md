﻿A time series value is a list of values that comprise the time series. At least one value must be supplied. Applications are expected to normalize values by applying the following three rules:

* All time (universal, local, daylight savings, and solar) is normalized against the ISO 8601 standard GMT/UTC (Universal Coordinated Time).
* Any rollover is handled by the application providing the data. Rollover occurs, for example, when the measurement device resets itself while measuring and the recording data do not include the data measured before the reset.
* The normalized data refer to the preceding time unit. The time series example shown in the figure below contains four time points: Time "a" indicates the beginning of the time series and the associated datum has no relevance. Data at time points "b," "c" and "d" are associated with values 1, 2 and 3, respectively.

<table> 
	<tr> 
	  <td valign="TOP" align="LEFT">
      </td> 
	  <td valign="TOP" align="LEFT">
        <img src="figures/ifctimeseries_timeseriesvalue.gif" alt="time series values" width="575" height="95" border="0">
        </td> 
	</tr> 
	</table>

> <font color="#0000FF" size="-1">
		<p>
    	HISTORY: New entity in IFC 2x2.<br>
	    </p>
    	</font>