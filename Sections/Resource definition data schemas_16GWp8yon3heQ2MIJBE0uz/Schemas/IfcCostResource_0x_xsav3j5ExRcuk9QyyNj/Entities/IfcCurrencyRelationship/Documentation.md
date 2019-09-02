An _IfcCurrencyRelationship_ defines the rate of exchange that applies between two designated currencies at a particular time and as published by a particular source.

> <font color="#0000FF" size="-1">HISTORY: New Entity in IFC
		2x2.</font>

### Use Definitions
An _IfcCurrencyRelationship_ is used where there may be a need to reference an IfcCostValue in one currency to an IfcCostValue in another currency. It takes account of fact that currency exchange rates may vary by requiring the recording the date and time of the currency exchange rate used and the source that publishes the rate. There may be many sources and there are different strategies for currency conversion (spot rate, forward buying of currency at a fixed rate).

The source for the currency exchange is defined as an instance of IfcLibraryInformation that includes a name and a location (typically a URL, since most rates are now published in reliable sources via the web, although it may be a string value defining a location of any type).