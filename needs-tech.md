# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given that I have a backup mechanism that copies the data
  into a secondary database every hour
  When a problem occurs and restarting the server is required
  Then I can recover all the lost data from secondary database

Scenario: Reconcile counts if the sensor is offline for a while

  Given that there is a mechanism to restore count
  from a secondary storage
  When the sensor goes offline
  Then I can reconcile the counts from the secondary storage
