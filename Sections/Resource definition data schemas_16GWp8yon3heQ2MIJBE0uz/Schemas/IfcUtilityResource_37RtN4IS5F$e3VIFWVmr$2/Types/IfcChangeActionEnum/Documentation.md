Enumeration identifying the type of change that might have occurred to the object during the last session (e.g., unchanged, added, deleted, etc.). This information is required in a partial model exchange scenario so that an application or model server will know how an object might have been affected by the previous application. Valid enumerations are:

* **NOCHANGE**: Object has not been modified. This is the default state.
* **MODIFIED**: A modification to the object has been made by the user and application defined by the LastModifyingUser and LastModifyingApplication respectively.
* **ADDED**: The object has been added by the user and application defined by the LastModifyingUser and LastModifyingApplication respectively.
* **DELETED**: The object has been deleted by the user and application defined by the LastModifyingUser and LastModifyingApplication respectively.
* **MODIFIEDADDED**: The object has been added and modified by the user and application defined by the LastModifyingUser and LastModifyingApplication respectively.
* **MODIFIEDDELETED**: The object has been modified and deleted by the user and application defined by the LastModifyingUser and LastModifyingApplication respectively.

Note that only the first four enumerations should be used. The MODIFIEDADDED and MODIFIEDDELETED are left for compatibility purposes but should not be used.

Consider Application A receives an IFC dataset, adds a new object and sets _IfcChangeActionEnum_ to ADDED. Application B then receives this IFC dataset but doesn't do anything to the object added by Application A. Consequently, the object's _IfcChangeActionEnum_ remains set at ADDED. Consequently, the intent is that an application only modifies the value of _IfcChangeActionEnum_ when it does something to the object, with the further intent that a model server is responsible for clearing the _IfcChangeActionEnum_ back to UNCHANGED when it is checked back into the repository.

> <font color="#0000FF" size="-1">
		<p>
    	HISTORY: New enumeration in IFC R2.0.<br>
	    </p>
    	</font>