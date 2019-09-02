Instances of _IfcCostItem_ are used for cost estimates, budgets, and other forms, where a variety of identification codes are used extensively to identify the meaning of the cost. Examples include project phase codes, CSI codes, takeoff sequence numbers, and cost accounts. The model allows for all classes that are ultimately subtypes of _IfcObject_ to inherit the ability to have one or more instances of _IfcClassificationReference_ to be assigned. Where identification codes are required, the generic _IfcRelAssociatesClassification_ facility should be used.