A zone (_IfcZone_) is an aggregation of spaces, partial spaces or other zones. Zone structures may not be hierarchical (in contrary to the spatial structure of a project - see _IfcSpatialStructureElement_), i.e. one individual _IfcSpace_ may be associated with zero, one, or several _IfcZone_'s. _IfcSpace_'s are aggregated into an _IfcZone_ by using the objectified relationship _IfcRelAssignsToGroup_ as specified at the supertype _IfcGroup_.

> <small>NOTE  Certain use cases may restrict the freedom
        of non hierarchical relationships. In some building
        service use cases the zone denotes a view based delimited
        volume for the purpose of analysis and calculation. This
        type of zone cannot overlap with respect to that
        analysis, but may overlap otherwise.</small>

> <small>NOTE  One of the purposes of a zone is to
        define a fire compartmentation. In this case it defines
        the geometric information about the fire compartment
        (through the contained spaces) and information, whether
        this compartment is ventilated or sprinkler protected. In
        addition the fire risk code and the hazard type can be
        added, the coding is normally defined within a national
        fire regulation. All that information is available within
        the relevant property sets.</small>

> <small>RECOMMENDATION  In case of a zone
        denoting a (fire) compartment, the following types should
        be used, if applicable, as values of the
        <i>ObjectType</i> attribute:</small><ul>
        <li>
          <small>FireCompartment - a zone of spaces,
          collected to represent a single fire
          compartment.</small>
        </li>
        <li>
          <small>ElevatorShaft - a collection of spaces
          within an elevator, potentially going through many
          storeys.</small>
        </li>
        <li>
          <small>RisingDuct</small>
        </li>
        <li>
          <small>RunningDuct</small>
        </li>
      </ul>

Additional classifications of the _IfcZone_, as provided by a national classification system, can be assigned by using the _IfcRelAssociatesClassification_ relationship.

> <small><font color="#0000FF">HISTORY New entity in IFC
        Release 1.0</font></small>

****Property Set Use Definition****:

The property sets relating to the _IfcZone_ are defined by the _IfcPropertySet_ and attached by the _IfcRelDefinesByProperties_ relationship. It is accessible by the inverse _IsDefinedBy_ relationship. The following property set definitions specific to the _IfcZone_ are part of this IFC release:

*  [Pset_ZoneCommon](../../psd/IfcProductExtension/Pset_ZoneCommon.xml){ target="SOURCE"}: common property set for all types of zone 
*  [Pset_SpaceFireSafetyRequirements](../../psd/IfcProductExtension/Pset_SpaceFireSafetyRequirements.xml){ target="SOURCE"}: common property set for all types of zones to capture the fire safety requirements 
*  [Pset_SpaceLightingRequirements](../../psd/IfcProductExtension/Pset_SpaceLightingRequirements.xml){ target="SOURCE"}: common property set for all types of zones to capture the lighting requirements 
*  [Pset_SpaceOccupancyRequirements](../../psd/IfcProductExtension/Pset_SpaceOccupancyRequirements.xml){ target="SOURCE"}: common property set for all types of zones to capture the occupancy requirements 
*  [Pset_SpaceThermalRequirements](../../psd/IfcProductExtension/Pset_SpaceThermalRequirements.xml){ target="SOURCE"}: common property set for all types of zones to capture the thermal requirements