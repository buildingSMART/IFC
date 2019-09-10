**Definition from ISO/CD 10303-42:1992**: A poly loop is a loop with straight edges bounding a planar region in space. A poly loop is a loop of genus 1 where the loop is represented by an ordered coplanar collection of points forming the vertices of the loop. The loop is composed of straight line segments joining a point in the collection to the succeeding point in the collection. The closing segment is from the last to the first point in the collection.&nbsp;

The direction of the loop is in the direction of the line segments.

> <small>NOTE &nbsp;This entity
exists primarily to facilitate the efficient communication of faceted
B-rep models. </small>

A poly loop shall conform to the following topological constraints:

<dl>
  <dd>- the loop has the genus of one.</dd>
  <dd>- the following equation shall be satisfied
    <dl>
      <dd> <img src="figures/ifcpolyloop-math1.gif" height="26" width="138"></dd>
    </dl>
  </dd>
</dl>&nbsp;The _IfcPolyLoop_ is always closed and the last segment is from the last _IfcCartesianPoint_ in the list of _Polygon_'s to the first _IfcCartesianPoint_. Therefore the first point shall not be repeated at the end of the list, neither by referencing the same instance, nor by using an additional instance of&nbsp;_IfcCartesianPoint_ having the coordinates as the first point.&nbsp;

> <small><font color="#0000ff">NOTE
&nbsp;
Corresponding STEP entity: poly_loop. Please refer to ISO/IS
10303-42:1994, p. 138 for the final definition of the formal standard.
Due to the general IFC model specification rule not to use multiple
inheritance, the subtype relationship to geometric_representation_item
is not included. The derived attribute <i>Dim</i> has been
added at this
level. <br>
  <br>
HISTORY &nbsp;
New class in IFC Release 1.0 </font></small>
> 


Informal propositions:

1. All the points in the polygon defining the poly loop shall be coplanar.
2. The first and the last _Polygon_ shall be different by value.
