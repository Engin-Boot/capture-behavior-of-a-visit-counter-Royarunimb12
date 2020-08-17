# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given server contains data recovery software
  When programmer restarts server or forcefully restarts server
  Then recover visit-counter from data recovery software

Scenario: Reconcile counts if the sensor is offline for a while

  Given server was online before turning offline and contains data recovery software 
  When server turns offline after it was online
  Then compare the new value of counts with what data recovery software delivers
