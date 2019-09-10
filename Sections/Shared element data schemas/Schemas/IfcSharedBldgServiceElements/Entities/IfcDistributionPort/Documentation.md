The product _IfcDistributionPort_ defines the occurrence of a specialized port for use within the context of distribution elements. Its type is defined by _IfcDistributionPortType_ or its subtypes.

****Property Set Use Definition****:

The property sets relating to this entity are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to this entity are part of this IFC release:

* [Pset_DistributionPortDuct](../../psd/IfcSharedBldgServiceElements/Pset_DistributionPortDuct.xml){ target="SOURCE"}: property set for duct distribution port occurrences 
* [Pset_DistributionPortPipe](../../psd/IfcSharedBldgServiceElements/Pset_DistributionPortPipe.xml){ target="SOURCE"}: property set for pipe distribution port occurrences 

> <font color="#0000ff" size="-1">
        HISTORY: New entity in IFC 2x2.
    </font>

**Use Definitions**

The images below will help present the concepts of how an _IfcDistributionPort_ is used to connect occurrences together in a distribution system. These concepts will be exemplified using a duct segment connecting to a tee and distributing air out through two connecting duct segments, as shown below in Figure 1.

<table border="0" cellpadding="0" width="100%">
 <tr>
  <td align="center">
  <p><img border="0" src="figures/ifcdistributionport_conceptslide3.gif" alt="Figure 1"></p>
  </td>
 </tr>
 <tr>
  <td align="center">
<blockquote>
    <font color="#0000ff" size="-1">
	<p>Figure 1: A tee distributing air out
  through two connecting duct segments</p>
    </font>
</blockquote>
  </td>
 </tr>
</table>

For the duct segments in this example, the concepts of the type, occurrence and performance history entities would be modeled using the following instances and shown in Figure 2:

* The type (and representation) is defined using _IfcDuctSegmentType_ from the _IfcHvacDomain_ schema
* The occurrences (and placements) are defined using _IfcFlowSegment_ from the _IfcSharedBldgServicesDomain_ schema
* The performance history characteristics for these occurrence are defined using _IfcPerformanceHistory_ from the _IfcControlExtension_ schema

<table border="0" cellpadding="0" width="100%">
 <tr>
  <td align="center">
  <p><img border="0" src="figures/ifcdistributionport_conceptslide4.gif" alt="Figure 2"></p>
  </td>
 </tr>
 <tr>
  <td align="center">
<blockquote>
    <font color="#0000ff" size="-1">
	<p>Figure 2: IFC entities used to represent a duct segment</p>
    </font>
</blockquote>
  </td>
 </tr>
</table>

The fitting would be represented in a similar manner using instances of _IfcDuctFittingType_, _IfcFlowFitting_ and _IfcPerformanceHistory_ for the type, occurrence and performance history entities respectively. Figure 3 includes all the type and occurrence entities that are involved in the duct and fitting example, as well as how the property sets defining type are related. Also included is how a port is involved in the connectivity of these entities.

<table border="0" cellpadding="0" width="100%">
 <tr>
  <td align="center">
  <p><img border="0" src="figures/ifcdistributionport_conceptslide5.gif" alt="Figure 3"></p>
  </td>
 </tr>
 <tr>
  <td align="center">
<blockquote>
    <font color="#0000ff" size="-1">
	<p>Figure 3: IFC entities used to represent the full example, 

including ports</p>
    </font>
</blockquote>
  </td>
 </tr>
</table>

If we look specifically at the point in the example where the duct segment connects to the inlet of the tee fitting, as shown in Figure 4, there is a port on the duct and a port on the tee which are used to logically relate the two together so that a connection is inferred. This connection may be physically realized with a specific fitting that is used to physically connect the duct segment and the tee fitting, such as a flange or coupling.   
It is important to note that the notion of a port is different from that of a connector.

<table border="0" cellpadding="0" width="100%">
 <tr>
  <td align="center">
  <p><img border="0" src="figures/ifcdistributionport_conceptslide6.gif" alt="Figure 4"></p>
  </td>
 </tr>
 <tr>
  <td align="center">
<blockquote>
    <font color="#0000ff" size="-1">
	<p>Figure 4: The relationships between distribution elements, 

ports and connectors</p>
    </font>
</blockquote>
  </td>
 </tr>
</table>

Figure 5 indicates how fluid flow properties and connection-specific information may be incorporated at the mass-flow boundary layers within this example.

<table border="0" cellpadding="0" width="100%">
 <tr>
  <td align="center">
  <p><img border="0" src="figures/ifcdistributionport_conceptslide7.gif" alt="Figure 5"></p>
  </td>
 </tr>
 <tr>
  <td align="center">
<blockquote>
    <font color="#0000ff" size="-1">
	<p>Figure 5: Modeling mass-flow characteristics across boundary 

layers</p>
    </font>
</blockquote>
  </td>
 </tr>
</table>