The type of signal modification effected and applicable ports:

LOWERLIMITSWITCH: Single analog input is read and if less than Value.LowerBound then True is written to the output value.
UPPERLIMITSWITCH: Single analog input is read and if more than Value.UpperBound then True is written to the output value.
LOWERBANDSWITCH: Single analog input is read and if less than Value.LowerBound+BandWidth then True is written to the output value.
UPPERBANDSWITCH: Single analog input is read and if more than Value.UpperBound-BandWidth then True is written to the output value.
NOT: Single binary input is read and the opposite value is written to the output value.
AND: Two binary inputs are read and if both are True then True is written to the output value.
OR: Two binary inputs are read and if either is True then True is written to the output value.
XOR: Two binary inputs are read and if one is true then True is written to the output value.
CALENDAR: No inputs; the current time is compared with an IfcWorkCalendar to which the IfcController is assigned and True is written if active.
INPUT: Controller element is a dedicated input.
OUTPUT: Controller element is a dedicated output.
VARIABLE: Controller element is an in-memory variable.
