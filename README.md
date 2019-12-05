# CP320-ExplorationProject

## Overview
This project will provide the code and wiring necessary to turn on the LED's and cycle through the columns with different colours.
It has one PWM signal going to the rows for the red LED's and another PWM signal going to the rows for the green LED's. There are also white LED's going from the Pi to the LED Matrix's columns and controls which column will be turned on at a time.


## Libraries Needed
The only libraries needed are the time library and the RPi.GPIO library


## Challenges
The biggest challenge for making this project was figuring out a way to get around the limitation on the number of GPIO pins available on the Raspberry Pi. This was solved by having all the rows be connected and only controlling the columns.


## Useful Links
[This link has the datasheet for the LED Matrix used. It has the pinouts and the recommended voltage for correct operation.](
http://denethor.wlu.ca/projects/sensors/LPT2558AA.pdf)

[This link has information on how to turn on a led with some more resources on controlling them from an arduino so you can have some more info on led control and led operation.](http://www.circuitbasics.com/arduino-basics-controlling-led/)

[This link has the GPIO pinout for the Raspberry Pi 2 which was the model I used. If you have the same model, you can use this pinout, otherwise you can find the pinout of your model and try to match the pins with the type of pins I used.](https://learn.sparkfun.com/tutorials/raspberry-gpio/gpio-pinout)
