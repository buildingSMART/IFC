{ .std}
## 3.1 Terms and definitions{#general-terms .std}
{ .std}
For the purpose of this document, the following definitions apply.

{ .std}
**attribute**{#attribute}

{ .std}
unit of information within an [entity](#entity){ .int-ref}, defined by a particular [type](#type){ .int-ref} or reference to a particular [entity](#entity){ .int-ref}

1. NOTE&nbsp; There are three kinds of attributes: [direct attributes](#attribute){ .int-ref}, [inverse attributes](#attribute){ .int-ref} and [derived attributes](#attribute){ .int-ref}. 

{ .std}
**direct
        attribute**{#direct-attribute}

{ .std}
scalar values or collections including Set (unordered, unique), List (ordered), or Array (ordered, sparse) as defined in [[ISO 10303-11]](chapter-2.htm#iso-10303-11){ .int-ref}

1. NOTE&nbsp; Similar to the term "field" in common programming languages. 

{ .std}
**inverse
        attribute**{#inverse-attribute}

{ .std}
unit of information defining queries for obtaining related data and enforcing referential integrity

1. NOTE&nbsp; Similar to the term "navigation property" in entity-relational programming frameworks. 

{ .std}
**derived
        attribute**{#derived-attribute}

{ .std}
unit of information computed from other attributes using an expression defined in the schema

{ .std}
**constraints on
        attributes**{#constraints-on-attribute}

{ .std}
data type restricting the values of attributes

1. NOTE&nbsp;1&nbsp; The most general constraint is about the existence of attribute values. There are basically two types: mandatory and optional attributes. Values of mandatory attributes must be provided whereas values of optional attributes may be omitted. 
2. NOTE&nbsp;2&nbsp; For aggregation data types such as Set, List, or Array, the existence constraint is often refined by a minimal and maximal number of elements, which is also known as cardinality. 

{ .std}
**entity**{#entity}

{ .std}
class of information defined by common [attributes](#attribute){ .int-ref} and constraints as defined in [[ISO 10303-11]](chapter-2.htm#iso-10303-11){ .int-ref}

1. NOTE&nbsp; Similar to the term "class" in common programming languages but describing data structure only (not behavior such as methods). 

{ .std}
**identification**{#identification}

{ .std}
capability to find, retrieve, report, change, or delete specific instances without ambiguity

{ .std}
**instance**{#instance}

{ .std}
occurrence of an entity

1. NOTE&nbsp; Similar to the term "instance of a class" in object oriented programming. 

{ .std}
**object**{#object}

{ .std}
anything perceivable or conceivable that has a distinct existence, albeit not material

{ .std}
**type**{#type}

{ .std}
basic information construct derived from a primitive, an [enumeration](#enumeration){ .int-ref}, or a [select](#select){ .int-ref} of entities

1. NOTE&nbsp;1&nbsp; Similar to the "Type" construct as defined in [[ISO 10303-11]](chapter-2.htm#iso-10303-11){ .int-ref}. 
2. NOTE&nbsp;2&nbsp; Similar in concept to "typedef" or "value type" in common programming languages. 

{ .std}
**select**{#select}

{ .std}
construct that allows an attribute value to be one of multiple [types](#type){ .int-ref} or [entities](#entity){ .int-ref}

1. NOTE&nbsp;1&nbsp; Similar to the "Select" construct as defined in [[ISO 10303-11]](chapter-2.htm#iso-10303-11){ .int-ref}. 
2. NOTE&nbsp;2&nbsp; Similar to a "marker interface" in common programming languages. 

{ .std}
**enumeration**{#enumeration}

{ .std}
construct that allows an attribute value to be one of multiple predefined values identified by name

1. NOTE&nbsp;1&nbsp; Similar to the "Enumeration" construct as defined in [[ISO 10303-11]](chapter-2.htm#iso-10303-11){ .int-ref}. 
2. NOTE&nbsp;2&nbsp; Similar in concept to "enum" in common programming languages. 

{ .std}
**actor**{#actor}

{ .std}
person, an organization, or person acting on behalf of an organization

1. NOTE&nbsp; A specialization of the general term [object](#object-type){ .int-ref}. 

{ .std}
**classification**{#classification}

{ .std}
categorization, the act of distributing things into classes or categories of the same type

{ .std}
**constraint**{#constraint}

{ .std}
restriction for a specified reason

1. NOTE&nbsp; A specialization of the general term [control](#control){ .int-ref}. 

{ .std}
**control**{#control}

{ .std}
directive to meet specified requirements such as for scope, time, and/or cost

1. NOTE&nbsp; A specialization of the general term [object](#object-type){ .int-ref}. 

{ .std}
**dictionary**{#dictionary}

{ .std}
collection of words, terms or concepts, with their definition

{ .std}
**element**{#element}

{ .std}
tangible physical product that can be described by its shape representation, material representations, and other properties

1. NOTE&nbsp; A specialization of the general term [product](#product){ .self-ref}. 

{ .std}
**element
        occurrence**{#element-occurrence}

{ .std}
element's position within the project coordinate system and its containment within the spatial structure

{ .std}
**external
        reference**{#external-reference}

{ .std}
link to information outside the data set, with direct relevance to the specific information the link originates from inside the data set

{ .std}
**feature**{#feature}

{ .std}
parametric information and additional property information modifiying the shape representation of an [element](#element){ .int-ref} to which it applies

{ .std}
**group**{#group}

{ .std}
collection of information that fulfills a specified purpose

1. NOTE&nbsp; A specialization of the general term [object](#object-type){ .int-ref}. 

{ .std}
**library**{#library}

{ .std}
catalogue, database or holder of data, that is relevant to information in the data set

1. NOTE&nbsp; It is information referenced from an external source that is not copied into the data set. 

{ .std}
**object
        occurrence**{#object-occurrence}

{ .std}
characteristics of an [object](#object-type){ .int-ref} as an individual

1. NOTE&nbsp; Similar to "object", "instance", "individual" in other publications. 

{ .std}
**object type**{#object-type}

{ .std}
common characteristics shared by multiple [object-occurrence](#object-occurrence){ .int-ref}s

1. NOTE&nbsp; Similar to "class", "template", "type" in other publications. 

{ .std}
**process**{#process}

{ .std}
[object-occurrence](#object-occurrence){ .int-ref} located in time, indicating "when"

{ .std}
**process
        occurrence**{#process-occurrence}

{ .std}
conceptual [object](#object-type){ .int-ref} that may occur at a particular time

{ .std}
**process type**{#process-type}

{ .std}
common characteristics shared by multiple [process occurrence](#process-occurrence){ .int-ref}s

{ .std}
**product**{#product}

{ .std}
physical or conceptual [object](#object){ .int-ref} that occurs in space

1. NOTE&nbsp; It is specialization of the general term [object](#object){ .int-ref}. 

{ .std}
**product
        occurrence**{#product-occurrence}

{ .std}
physical or conceptual [object](#object){ .int-ref} that may have a location in space and shape characteristics

{ .std}
**product type**{#product-type}

{ .std}
common characteristics shared by multiple [product occurrence](#product-occurrence){ .int-ref}s

{ .std}
**project**{#project}

{ .std}
encapsulation of related information for a particular purpose providing context for information contained within

1. NOTE&nbsp; Context information may include default measurement units or representation context and precision. 

{ .std}
**property**{#property}

{ .std}
unit of information that is dynamically defined as a particular [entity](#entity){ .int-ref} instance

1. NOTE&nbsp; Similar to "late-bound" or "run-time" in programming terminology. 

{ .std}
**property
        occurrence**{#property-occurrence}

{ .std}
unit of information providing a value for a [property](#property){ .int-ref} identified by name

{ .std}
**property
        template**{#property-template}

{ .std}
metadata for a [property](#property){ .int-ref} including name, description, and data type

1. NOTE&nbsp; Similar in concept to "extension property" in common programming languages. 

{ .std}
**property set occurrence**{#property-set-occurrence}

{ .std}
unit of information containing a set of [property occurrence](#property-occurrence){ .int-ref}s, each having a unique name within the property set

{ .std}
**property
        set template**{#property-set-template}

{ .std}
set of [property
        template](#property-template){ .int-ref}s serving a common purpose and having applicability to [object](#object){ .int-ref}s of a particular [entity](#entity){ .int-ref}

1. NOTE&nbsp; Similar in concept to "extension class" in common programming languages. 

{ .std}
**proxy**{#proxy}

{ .std}
object that does not hold a specific [object type](#object-type){ .int-ref} information

1. NOTE&nbsp; a specialization of [object occurrence](#object-occurrence){ .int-ref}. 

{ .std}
**quantity**{#quantity}

{ .std}
measurement of a scope-based metric, specifically length, area, volume, weight, count, or time

{ .std}
**quantity
        occurrence**{#quantity-occurrence}

{ .std}
unit of information providing a value for a [quantity](#quantity){ .int-ref}

{ .std}
**quantity set**{#quantity-set}

{ .std}
unit of information containing a set of [quantity occurrence](#quantity-occurrence){ .int-ref}s, each having a unique name within the quantity set

{ .std}
**relationship**{#relationship}

{ .std}
unit of information describing an interaction between items

{ .std}
**representation**{#representation}

{ .std}
unit of information describing how an object is displayed, such as physical shape or topology

{ .std}
**resource**{#resource}

{ .std}
entity with limited availability such as materials, labor, or equipment

1. NOTE&nbsp;1&nbsp; a specialization of the general term [object](#object-type){ .int-ref}. 
2. NOTE&nbsp;2&nbsp; the "resource definition data schemas" section is unrelated to this concept. 

{ .std}
**resource
        occurrence**{#resource-occurrence}

{ .std}
entity with inherent financial cost, which may be passed onto [processes](#process){ .int-ref}, [products](#product){ .int-ref}, and [controls](#control){ .int-ref} to which it is assigned

{ .std}
**resource type**{#resource-type}

{ .std}
common characteristics shared by multiple [resource occurrence](#resource-occurrence){ .int-ref}s

{ .std}
**space**{#space}

{ .std}
area or volume bounded actually or theoretically

1. NOTE&nbsp; a specialization of the general term [product.](#product){ .self-ref} 

{ .std}
## 3.2 Abbreviated terms{#abbrevated-terms}
{ .std}
For the purpose of this document, the following abbreviated terms apply:

{ .std}
<table class="std" summary="Abbreviated terms" title="Abbreviated terms">
        <col width="100px">
        <col>
        <tr>
          <td class="std">
            <a id="aec" name="aec">AEC</a>
          </td>
          <td class="std">
            Architecture, Engineering, and Construction
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="aec-fm" name="aec-fm">AEC/FM</a>
          </td>
          <td class="std">
            Architecture, Engineering, Construction, and Facilities Management
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="bim" name="bim">BIM</a>
          </td>
          <td class="std">
            Building Information Modeling
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="guid" name="guid">GUID</a>
          </td>
          <td class="std">
            Globally Unique Identifier
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="ifc" name="ifc">IFC</a>
          </td>
          <td class="std">
            Industry Foundation Classes
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="ifd" name="ifd">IFD</a>
          </td>
          <td class="std">
            International Framework for Dictionaries
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="spf" name="spf">SPF</a>
          </td>
          <td class="std">
            STEP Physical File
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="step" name="step">STEP</a>
          </td>
          <td class="std">
            STandard for the Exchange of Product data
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="uri" name="uri">URI</a>
          </td>
          <td class="std">
            Uniform Resource Identifier
          </td>
        </tr>
        <tr>
          <td class="std">
            <a id="uuid" name="uuid">UUID</a>
          </td>
          <td class="std">
            Universally Unique Identifier
          </td>
        </tr>
      </table>
