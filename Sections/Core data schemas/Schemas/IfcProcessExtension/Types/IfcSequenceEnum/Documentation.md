_IfcSequenceEnum_ is an enumeration that defines the different ways in which a time lag is applied to a sequence between two processes.

> HISTORY&nbsp; New entity in IFC1.0

{ .spec-head}
Enumerated Item Definitions:

<lu>
      <li><b>FINISH_START</b>: The predecessor task must finish before the successor task may start.</li>
      <li><b>FINISH_FINISH</b>: The predecessor task must finish before the successor task may finish.</li>
      <li><b>START_START</b>: The predecessor task must start before the successor task may start.</li>
      <li><b>START_FINISH</b>: The predecessor task must start before the successor task may finish.</li>
    </lu>