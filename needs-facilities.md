# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given I have a dashboard to plot a graph between two pairs of values
  When I update the number of visitors per day against
  the day on everyday in a week
  Then I can see the trend of visitors in any given week

Scenario: Alert when seating capacity is full

  Given I have a threshold value and a system
  monitoring the seating capacity
  When the seating capacity becomes greater than the
  threshold at any point of time
  Then I can have an alert to inform me about seating capacity
