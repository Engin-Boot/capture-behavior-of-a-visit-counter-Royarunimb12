# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given data recovery software is installed in server
  When server restarts or forceful restart
  Then recover visit-counter from data recovery software

Scenario: Reconcile counts if the sensor is offline for a while

  Given
  When
  Then
