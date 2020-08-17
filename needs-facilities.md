# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given hospital is functional
  When there is movement at the entry
  Then plot statistics on graph

Scenario: Alert when seating capacity is full

  Given hospital is functional
  When number of empty seats is equal to 0
  Then send alert to system
