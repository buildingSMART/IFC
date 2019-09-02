The flight foot print, including the flight boundary is represented by a two-dimensional geometric curve set.

Figure 1 illustrates the footprint representation which has the following constraints:

* In case of straight flights the curve set shall consist of a single item of type _IfcPolyline_.
* In case of winding flights or curved flights the curve set shall consists of a single item of type _IfcCompositeCurve_.
* In case of a spiral flight the curve set shall consists of a single item of type _IfcConic_ or _IfcPolyline_.

!["boundary"](../../../figures/IfcStairFlight_02-Layout1.gif "Figure 1 &mdash; Ramp flight footprint")