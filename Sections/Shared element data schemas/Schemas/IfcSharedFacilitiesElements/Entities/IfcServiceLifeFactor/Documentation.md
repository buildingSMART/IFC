An _IfcServiceLifeFactor_ captures the various factors that impact upon the expected service life of an artefact.

> <font size="-1" color="#0000FF">HISTORY: New entity in IFC
		2x2</font>

### Use Definitions
Note that each instance of _IfcServiceLifeFactor_ may have a name that describes the form of impact that the factor has on the service life. Because there is a significant list of such potential impacts, they are not explicitly collected together into an enumeration. In order to name an instance of _IfcServiceLifeFactor_, the inherited _Name_ attribute should be used.

Within the IFC specification, any number of service life factors may be allowed to impact upon the service life of an artefact. In many cases, it is probable that the ISO standard that specifies good practice for service life consideration will be applied.

Within the ISO standard, there are seven defined (named) service life factors that may be applied to an _IfcServiceLife_. These are captured in the IfcServiceLifeFactorEnum (together with a user defined capability). Each factor can have three values that define an upper, lower and most used (or median) value.

One or more instances of _IfcServiceLifeFactor_ can be related to an _IfcServiceLife_ through the _IfcRelDefinesByProperties_ relationship class.
