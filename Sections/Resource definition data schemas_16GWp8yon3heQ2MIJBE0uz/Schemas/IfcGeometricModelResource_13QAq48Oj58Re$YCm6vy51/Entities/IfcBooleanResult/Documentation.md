**Definition from ISO/CD 10303-42:1992**: A Boolean result is the result of a regularized operation on two solids to create a new solid. Valid operations are regularized union, regularized intersection, and regularized difference. For purpose of Boolean operations, a solid is considered to be a regularized set of points. The final Boolean result depends upon the operation and the two operands. In the case of the difference operator the order of the operands is also significant. The operator can be either union, intersection or difference. The effect of these operators is described below:

* Union on two solids is the new solid that is the regularization of the set of all points that are in either the first operand or the second operand or in both. 
* Intersection on two solids is the new solid that is the regularization of the set of all points that are in both the first operand and the second operand. 
* The result of the difference operation on two solids is the regularization of the set of all points which are in the first operand, but not in the second operand. 

> <font color="#0000FF" size="-1">NOTE Corresponding STEP entity:
		  boolean_result. The derived attribute <i>Dim</i> has been added at this level
		  and was therefore demoted from the geometric_representation_item. Please refer
		  to ISO/IS 10303-42:1994, p.175 for the final definition of the formal standard.
		  </font>
> 
> <font color="#0000FF" size="-1">HISTORY: New class in IFC Release
		  1.5.1.</font>
>