# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given server contains data recovery software
  When programmer restarts server or forcefully restarts
  Then recover visit-counter from data recovery software

Scenario: Reconcile counts if the sensor is offline for a while

  Given
  When
  Then
