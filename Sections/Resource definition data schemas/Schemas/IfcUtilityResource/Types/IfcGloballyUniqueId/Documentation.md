Holds an identifier that is unique throughout the software world. This is also known as a Globally Unique Identifier (GUID) or Universal Unique Identifier (UUID) by the Open Group. The identifier is generated using an algorithm published by the Object Management Group. The algorithm is explained at the open group [website](http://www.opengroup.org/dce/info/draft-leach-uuids-guids-01.txt). The Microsoft Foundation Class (MFC) function "CoCreateGuid", which is an implementation of the above algorithm, has been used by many IFC implementers to create an identifier.

An identifier is a unique 128-bit number. Since this identifier is required for all IFC object instances, it is desirable to compress the identifier size to reduce overhead. Beginning in IFC R1.5.1, IFC implementers agreed to compress the identifier down to 20 characters using an algorithm developed by IAI Implementers. This algorithm maps the identifier bits onto a base 85 digit encoded from the following character set:

0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz!#$%&amp;\^|\*+,-./:;&lt;=&gt;?\~`@_

An index (0-84) into this character set string determines the "value" for each character (e.g. "A" has a value of 10, "@" has a value of 83, etc.). Note that all characters are case-sensitive. In order to prevent possible problems with some parsers, implementers have agreed not to use the "/\*" and "\*/" character combinations in the identifier string and instead to use "\\*" and "\*\".

The implementation of the compression algorithm has changed in IFC R2x in order to prevent conflicts with special characters in the ISO 10303-21 exchange file and the W3C XML file (such as '&lt;\*', '\*&gt;', '&lt;' and '&gt;'). Using 64 characters for the base rather than 85, the resulting compressed string now needs 22 characters. The encoding of the base 64 character set is shown below:

> <font face="Courier New" size="-1">
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;6
		<br>&nbsp;0123456789012345678901234567890123456789012345678901234567890123<br>
		"0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz_$";
        </font>
> 


The following code example in C is given as a guideline for creating the base 64 compressed strings and for mapping the previous base 85 strings to the base 64 strings. This code is provided "as-is" with no support or guarantee of suitability provided by the IAI. Use of the code example is at the sole risk of the user.

* [CreateGuid_64.h](text/CreateGuid_64.h){ target="new"}
* [CreateGuid_64.c](text/CreateGuid_64.c){ target="new"}

The resulting string is a fixed 22 character length string to be exchanged within the IFC exchange file structure.

> <font size="-1" color="#0000FF">
    <p>
    	HISTORY: New type in IFC R1.5.1.<br>
	        </p>
	</font>