{ .extDef}
> Definition according to W3C for Cascading Style Sheets:  
> Setting font properties will be among the most common uses of style sheets. Unfortunately, there exists no well-defined and universally accepted taxonomy for classifying fonts, and terms that apply to one font family may not be appropriate for others. For example, 'italic' is commonly used to label slanted text, but slanted text may also be labeled as being _Oblique_, _Slanted_, _Incline_, _Cursive_ or _Kursiv_. Therefore it is not a simple problem to map typical font selection properties to a specific font.

{ .extDef}
> **Font matching**  
> Because there is no accepted, universal taxonomy of font properties, matching of properties to font faces must be done carefully. The properties are matched in a well-defined order to ensure that the results of this matching process are as consistent as possible across user agents (assuming that the same library of font faces is presented to each of them).

1. The user agent makes (or accesses) a database of relevant CSS1 properties of all the fonts of which the UA is aware. The UA may be aware of a font because it has been installed locally or it has been previously downloaded over the web. If there are two fonts with exactly the same properties, one of them is ignored. 
2. At a given element and for each character in that element, the UA assembles the font-properties applicable to that element. Using the complete set of properties, the UA uses the 'font-family' property to choose a tentative font family. The remaining properties are tested against the family according to the matching criteria described with each property. If there are matches for all the remaining properties, then that is the matching font face for the given element. 
3. If there is no matching font face within the 'font-family' being processed by step 2, and if there is a next alternative 'font-family' in the font set, then repeat step 2 with the next alternative 'font-family'. 
4. If there is a matching font face, but it doesn't contain a glyph for the current character, and if there is a next alternative 'font-family' in the font sets, then repeat step 2 with the next alternative 'font-family'.&nbsp; 
5. If there is no font within the family selected in 2, then use a UA-dependent default 'font-family' and repeat step 2, using the best match that can be obtained within the default font. 

(The above algorithm can be optimized to avoid having to revisit the CSS1 properties for each character.)

The per-property matching rules from (2) above are as follows:

1. 'font-style' is tried first. 'italic' will be satisfied if there is either a face in the UA's font database labeled with the CSS keyword 'italic' (preferred) or 'oblique'. Otherwise the values must be matched exactly or font-style will fail. 
2. 'font-variant' is tried next. 'normal' matches a font not labeled as 'small-caps'; 'small-caps' matches (1) a font labeled as 'small-caps', (2) a font in which the small caps are synthesized, or (3) a font where all lowercase letters are replaced by upper case letters. A small-caps font may be synthesized by electronically scaling uppercase letters from a normal font. 
3. 'font-weight' is matched next, it will never fail. (See 'font-weight' below.) 
4. 'font-size' must be matched within a UA-dependent margin of tolerance. (Typically, sizes for scalable fonts are rounded to the nearest whole pixel, while the tolerance for bitmapped fonts could be as large as 20%.) Further computations, are based on the 'font-size' value that is used, not the one that is specified.

The inherited _Name_ attribute is used to define the font name, particularly in cases, where no (list of) font families are provided.

> NOTE&nbsp; Corresponding CSS1 definitions are Font properties ('font-family', 'font-style', 'font-variant',&nbsp; 'font-weight').

> HISTORY&nbsp; New entity in IFC2x3.