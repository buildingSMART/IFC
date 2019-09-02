A medical device is attached to a medical piping system and operates upon medical gases to perform a specific function. Medical gases include medical air, medical vacuum, oxygen, carbon dioxide, nitrogen, and nitrous oxide.

Outlets for medical gasses should use _IfcValve_ with PredefinedType equal to GASTAP, containing an _IfcDistributionPort_ with FlowDirection=SINK and PredefinedType equal to COMPRESSEDAIR, VACUUM, or CHEMICAL, and having property sets on the port further indicating the gas type and pressure. Tanks for medical gasses should use _IfcTank_ with PredefinedType equal to PRESSUREVESSEL, containing an _IfcDistributionPort_ with FlowDirection=SOURCE and PredefinedType=CHEMICAL, and having property sets on the port further indicating the gas type and pressure range.

> HISTORY&nbsp; New entity in IFC4

{ .note}
>