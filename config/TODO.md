TODO:

* [ ] Flash rest of Mijia sensors
* [ ] Move secrets so Git exporter can run
* [x] Test magnet on gate opener to see if it marks it closed
* [ ] Fix gate opener
      Seems like the reed sensor is failing or the cable is damaged, so always reports open (holding magnet to it does not report closed :\)
* [ ] Cache volumes using dictionary as per https://community.home-assistant.io/t/remember-volume-levels-of-each-source-for-a-media-player-to-automate-restoring/416749/6?u=bjeanes
* [ ] Restore cache for volumes by using a `sql` sensor to read from DB
      (template sensors are not restored since they assume they are always calculated, but since it's mutually recursive it does rely on the running state to be accurate)