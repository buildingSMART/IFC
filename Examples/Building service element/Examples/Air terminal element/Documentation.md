This example includes a building file containing an air terminal occurrence referencing the external type. It demonstrates type instantiation, tapered extruded solid geometry, port connectivity, duct segments with material profiles, and library referencing.

The air terminal occurrence is placed within a building and has its inlet port connected to the outlet port of a duct segment. The air terminal occurrence has mapped geometry according to the type imported from the other file. The duct segment has an associated material profile set of an aluminum hollow circle, an 'Axis' representation indicating the path following a straight line upwards, and a 'Body' representation constructed by extruding the profile along the axis. The aluminum material has a surface style defined using a texture embedded within the file. Figure 1 illustrates the air terminal occurrence connected to the duct segment, where ports are not shown.

> NOTE&nbsp; The example contains an air terminal by itself for brevity; in an actual building, such air terminal would likely fill an opening of a ceiling covering within a space.

!["example of air terminal"](../../../../figures/examples/building_service_element_air-terminal-1.png "Figure 1 &mdash; Air terminal occurrence representation")

The air terminal occurrence is linked to the type using mapped geometry, as illustrated in Figure 2.

!["example of air terminal"](../../../../figures/examples/building_service_element_air-terminal-2.png "Figure 2 &mdash; Air terminal occurrence object graph")
