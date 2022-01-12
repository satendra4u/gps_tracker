# gps_tracker

This program uses the Tiny GPS module and they header file which has function to override.

#include "TinyGPS/TinyGPS.h"

This program also uses the Spark fun battery guage module to guage the battery and state of charge and sends the publish message if the battery is only 10% left.

The main GPS code runs in to the loop every 10 seconds get the latitude and longitude of the coordinates and also the speed.


      Particle.variable("gLatitude", &latitude, DOUBLE);

      Particle.variable("gLongitude", &longitude, DOUBLE);

      Particle.variable("gSpeed", &mSpeed, DOUBLE);

      To read the values from a browser, go to:
	    http://api.particle.io/v1/devices/{DEVICE_ID}/{VARIABLE}?access_token={ACCESS_TOKEN}

	    
