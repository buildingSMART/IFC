Enumeration identifying the state or accessibility of the object (e.g., read/write, locked, etc.). This concept was initially introduced in IFC 2.0 as _IfcModifiedFlag_ of type BINARY(3) FIXED and has been modified in R2x to an enumeration. It was initially introduced as a first step towards providing facilities for partial model exchange from a server as requested by the IFC implementers. It is intended for use primarily by a model server so that an application can identify the state of the object.

Valid enumerations are:

* **READWRITE**: Object is in a Read-Write state. It may be modified by an application.
* **READONLY**: Object is in a Read-Only state. It may be viewed but not modified by an application.
* **LOCKED**: Object is in a Locked state. It may not be accessed by an application.
* **READWRITELOCKED**: Object is in a Read-Write-Locked state. It may not be accessed by an application.
* **READONLYLOCKED**: Object is in a Read-Only-Locked state. It may not be accessed by an application.

> <font color="#0000FF" size="-1">
		<p>
    	HISTORY: New enumeration in IFC R2.0.<br>
	        </p>
    	</font>