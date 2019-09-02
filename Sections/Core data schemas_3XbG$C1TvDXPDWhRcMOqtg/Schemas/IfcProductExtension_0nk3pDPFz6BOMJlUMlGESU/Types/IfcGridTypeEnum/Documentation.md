This enumeration defines the different layout types of grids. Restriction on the correct use of _IfcGrid_ instantiations may be imposed depending on the value of the _PredefinedType_ being _IfcGridTypeEnum_.

> HISTORY&nbsp; New enumeration in IFC4.

**Enumeration**:

<ul>
      <li>
        <b>RECTANGULAR</b>:
        an <em>IfcGrid</em> with straight u-axes and straight
        v-axes being perpendicular to each other. All grid axes
        being part of u-axes can be described by one axis line and
        all other axes being 2D offsets from this axis line. The
        same applies to all grid axes being part of V-axes.
      </li>
      <li>
        <b>RADIAL</b>: an
        <em>IfcGrid</em> with straight u-axes and curved v-axes.
        All grid axes being part of V-axes have the same center
        point and are concentric circular arcs. All grid axes being
        part of u-axes intersect at the same center point and
        rotate counter clockwise.
      </li>
      <li>
        <b>TRIANGULAR</b>:
        an <em>IfcGrid</em> with u-axes, v-axes, and w-axes all
        being co-linear axis lines with a 2D offset. The v-axes are
        at 60 degree rotated counter clockwise from the u-axes, and
        the w-axes are at 120 degree rotated counter clockwise from
        the u-axes.
      </li>
      <li>
        <b>IRREGULAR</b>: an
        <em>IfcGrid</em> with u-axes, v-axes, and optionally w-axes
        that cannot be described by the patterns <span style="font-size:smaller; font-weight:bold;">RECTANGULAR, RADIAL,
        TRIANGULAR</span>.
        <blockquote class="note">
          NOTE&nbsp; Grids with irregular offsets between parallel
          or cocentric grid axes are not considered as <span style="font-size:smaller; font-weight:bold;">IRREGULAR</span>
          if they otherwise meet the criteria of <span style="font-size:smaller; font-weight:bold;">RECTANGULAR,
          RADIAL, TRIANGULAR</span>
        </blockquote>
      </li>
      <li>
        <b>USERDEFINED</b>:
        any other grid not conforming to any of the above
        restrictions;
      </li>
      <li>
        <b>NOTDEFINED</b>:
        not known whether grid conforms to any standard type.
      </li>
    </ul>
> NOTE&nbsp; View definitions or implementer agreements may impose further restrictions on how to populate the grid axes. The first grid axis being part of u-axes may have to be parallel to the x-axis of the grid object placement.