# Using two monitors at once

Some venues are able to build a second monitor or borrow one from another venue.   If you want to use two at the same time to send readings to the internet, there is a snag - the hub can't tell which sensor is which, so all the readings end up on the same ThingSpeak feed.  So far we have been able to separate the two sets of readings but it does take extra human effort, and we can't guarantee our technique will work in every circumstance.  **If you do this, please try to start the second sensor around 90 seconds after the first and ask us if you want us to do the separation.**

- [How Separation Works](https://jeancarletta.github.io/HeatHack-Extras/venue-10-reasoning.html)

A surer method is to convert the monitors to work in stand-alone mode.  Then you can use as many monitors as you can get.  You will then have to pick up the readings manually.  Read the stand-alone section of the guide and contact us if you wish to do this.   We don't have step-by-step instructions yet for this, but  for the tech-minded:

- power-cycle the sensor unit
- connect to the engineer wifi access point (password "heathack") 
- visit http://192.168.4.1/extra 
- first button lets you switch to Memory, then click on Submit.

After this, the steps are as in the stand-alone section, but you are already connected to the sensor's "engineer" wifi access point and just need to enter a location and start it recording by pressing Download and Start.  Do not omit the last step as this also copies the correct time from your phone to the sensor.


