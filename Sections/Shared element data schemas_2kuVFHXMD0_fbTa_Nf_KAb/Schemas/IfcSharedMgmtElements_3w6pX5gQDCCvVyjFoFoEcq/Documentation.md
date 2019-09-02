The _IfcSharedMgmtElements_ schema defines basic concepts that are common to management throughout the various stages of the building lifecycle. The primary classes in the schema are all subtypes of _IfcControl_ and act to manage or regulate the conduct of the project in some way. This schema, along with _IfcProcessExtension_ and _IfcConstructionMgmtDomain_, provide a set of models that can be used by applications needing to share information concerning management related issues.

## Scope
The objective of the IfcSharedMgmtElements schema is to capture information that supports the ordering of work and components, the development of cost schedules and the association of environmental impact information. The aim is to provide support for exchange and sharing of minimal information concerning the subjects in scope; the extent of the model will not support the more detailed ideas found in more specialized management applications.

The following are within the scope of this part of the specifications:

* Principal types of order that may be used in the project and whose details need to be captured for the project including purchase orders, change orders and work orders.
* Schedules of costs.
* Association of cost and environmental impact of information to specific objects as required.

The following are outside of the scope of this part of the specifications:

* Transaction details that may be supported by or support electronic commerce.

## Process Usage
### Project Orders
All types of order contain a basic set of attributes that enable the identification of the order, who it is issued by, who it is issued to and when it is issued. These are the fundamental requirements of an order.

Three types of project order are defined:

* Change Order
* Purchase Order
* Work Order

#### Change Order
The change order provides details of when an instruction is given to make a change in the project. It includes a description of the change and the reasons for it occurring. It may relate various documents to the change requirement. A change order will also have date/time constraints related; typically including such constraints as requested start and finish time, actual start and finish time (times at which the change is started and finished). Change orders may also have associated cost representations of various types, each representation being related through a single relationship. A work plan can also be associated in which the various tasks and resources required can be exposed.

#### Purchase Order
The purchase order can handle information concerning any type of purchase including both component and services purchases. Individual items within the purchase order are referenced from a cost representation that can identify individual costs. The purchase order also captures some information about logistics including shipping method (where a component is required).

#### Work Order
The work order provides a general approach to capturing information concerning an instruction given to do work. Various individual types of work order may be further defined in domain schema (e.g. maintenance work order).

### Cost Schedule
A cost schedule provides the means to bring together instances of _IfcCostScheduleItem_ as a budget, cost plan, estimate, tender, bill of quantities etc.

### Cost Schedule Item
A cost schedule item provides the means to define the individual items that form the complete cost schedule.