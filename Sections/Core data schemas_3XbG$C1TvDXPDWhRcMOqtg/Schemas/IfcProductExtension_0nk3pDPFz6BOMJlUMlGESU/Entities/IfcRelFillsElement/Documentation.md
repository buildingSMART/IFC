Objectified relationship between an opening element and an ~~building~~ element that fills (or partially fills) the opening element. It is an one-to-one relationship.

> <small>NOTE view definitions or implementer agreements
        may restrict an opening to be filled by one filling
        element only.</small>
> 


!["relationships for filling"](figures/IfcRelFillsElements-Fig1.png "<small><br>
          Figure  The insertion of a door into a wall is
          represented by two separate relationships. First the
          door opening is created within the wall by
          <i>IfcWall(StandardCase) o-- IfcRelVoidsElement --o
          IfcOpeningElement</i>, then the door is inserted within
          the opening by <i>IfcOpeningElement o--
          IfcRelFillsElement --o IfcDoor</i>.</small>")

> <small><font color="#0000FF">HISTORY New entity in IFC
        Release 1.0</font></small>
>