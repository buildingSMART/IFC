﻿An _IfcApproval_ represents information about approval processes such as for a plan, a design, a proposal, or a change order in a construction or facilities management project. _IfcApproval_ is referenced by _IfcRelAssociatesApproval_ in _IfcControlExtension_ schema, and thereby can be related to all subtypes of _IfcRoot_. An approval may also be given to resource objects using _IfcResourceApprovalRelationship_

> HISTORY&nbsp; New entity in IFC2.0

{ .change-ifc4}
> IFC4 CHANGE&nbsp; Attributes Identifier and Name made optional, where rule added to require at least one of them being asserted. Inverse attributes ApprovedObjects, ApprovedResources and HasExternalReferences added. Inverse attribute Properties deleted (more general relationship via inverse ApprovedResources to be used instead).
