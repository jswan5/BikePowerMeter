# BikePowerMeter
Building a strain gauge based meter to measure power from a stationary bike

Motivation:

It can be difficult to train for cycling when the weather is uncooperative. Though I have a couple of great bikes I can ride outdoors, and can quantify my training with sports watches, indoor training is tougher. The stationary bike I train on indoors gives no feedback for wattage, only a knob to adjust resistance. Therefore, can I implement some system that will allow me to quantify my work done on the bike, and measure progress?

EQUIPMENT:
1x Stationary Bike
1x Arduino UNO (deprecated)
1x ESP32WROOM-32
1x HX711 24-bit ADC
2x BF350-3AA strain gauge
1x (2x CR2032) battery case

Inspiration (and proof of concept, really) was drawn from the following webpages:

https://hackaday.com/2016/04/03/bike-power-meter-with-crank-mounted-wifi-strain-gauges/
http://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2014/mje56_bwc65/mje56_bwc65/index.html

The work was initially started in Arduino, with some potentially promising prototyping of the strain gauge setup: https://imgur.com/a/MaXUPIk

After hitting limitations of my knowledge in Arduino, I decided to move to microPython. It turned out to be much less intuitive, and much work is still required

TO-DO (in no particular order):

1. Find optimal setup for strain gauges (Wheatstone half bridge?)
2. Calibrate force production
3. Send force signal via Bluetooth
4. Find optimal power source (button cell batteries?)
5. Attach setup to cranks
6. Introduce native cadence (Hall sensor?)
