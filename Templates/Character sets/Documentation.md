**General concept template** regarding the whole IFC date set.

If the IFC data set is delivered as an STEP physical file (ISO 10303-21 format) non ASCII characters are required to be encoded according to the encoding instructions of ISO 10303-21.

Note: see the string encoding instruction published at [buildingsmart-tech.org](http://buildingsmart-tech.org/developers/get-started/string-encoding){ target="_blank"}

A Model View Definition shall specify which of the character encodings are required to be supported for a valid export, and are required to be read for import.

The encodings of non ASCII characters following the STEP physical file encoding include:

*  \S\,
*  \PA\, \PB\, ...&nbsp;
*  \X\,
*  \X2\...\X0\
