# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given that I have a counter mechanism
  When I update the counter for every incoming patient on each day
  Then I will be able to tell the number of patients who visited on any given day (working day or holiday)

Scenario: Compute parking slots to reserve for visiting specialists

  Given I have a digital map of the parking area with open slots in green color(ng), reserved slots in yellow(ny), and occupied slots in red color(nr) updated in realtime
  When I come to know that n number of specialists are visiting my hospital and take a minimum of n and ng
  Then I can calculate the number of slots that can be allocated to the specialists
