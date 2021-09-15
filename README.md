# DIY-Arduino-based-Touch-Free-Hand-sanitizer-dispenser

![image](https://user-images.githubusercontent.com/19898602/133388025-46fc443f-e816-4298-8a81-449c023bec7d.png)


n this current scenario of global outbreak, it is advised by WHO (world health organization) to maintain Healthy Hand Wash and Sanitation Habits, but the main problem is the way we do it, that is by physical touch to the bottle, which in short doesn’t serve our purpose, so in this tutorial, we will learn How To make a D.I.Y. Arduino Based Soap or Hand Sanitizer Dispenser.

![image](https://user-images.githubusercontent.com/19898602/133388780-f348b794-48db-4ba0-a5df-08dbbd16a0a7.png)


# COMPONENT USED

Arduino Nano ( or any Arduino ).
Ultrasonic Sensor ( HC-SR04)
Servo Motor ( metal Geared Preferred ).
Jumper Wires ( female to female )



First and the most important thing we will need for this build is Alcohol Based Hand Rub or Hand Sanitizer or Hand Wash as suggested by W.H.O. ( world health organization ) find more information here.

for this build, it is very important to get right kind of dispenser, since we are just making a dispenser and not printing the entire mechanism, we will need alcohol or hand rub in dispenser or push type bottle.


Sensor:

We will need a Sensor to sense our proximity or presence which will basically act as a trigger or touch less switch for this system. We have two choices here, that is we can use either IR sensor Module, or Ultrasonic sensor Module. We can use IR sensor Module, which is basically a cheap and efficient option, but sometimes inaccurate, or we can use HC-SR04 Ultrasonic sensor, which is quite accurate above 2 cm range, and slightly expensive option, but we will use Ultrasonic Sensor for this Tutorial, for better accuracy.

Motors:

For motion or to process the Output, we might need either a pump, either motor, or some electronic component that will convert electrical signal to mechanical displacement of alcohol based hand rub or sanitizer through the dispenser, best choice would be to use a Servo motor with metal gears for maximum torque. We will avoid using micro pumps, since they are to be inserted into the container, which again creates vulnerable containment spot. So using an external mechanism with help of servo would be a wise choice.

Microcontroller:

For this project build, we will need a Microcontroller to control the Input and Output, to Calculate the distance or sense the Trigger from Sensor and Process the Output in form of Servo Sweep in our Example, for which we can use any arduino, which makes it easy to adjust the parameters, fine tune outputs, so you can use any Arduino, we will use Arduino Nano for our work case.


# CIRCUIT DIAGRAM

![image](https://user-images.githubusercontent.com/19898602/133388267-38594e15-9e92-4d22-81ab-9c0f10a7e3b3.png)


Connections for this build is very simple !

Sensor to Arduino:

Trigger to D10

Echo to D11

Vcc to Vcc

Gnd to Gnd

Servo to Arduino:

Signal to D9

Vcc to Vin

Gnd to Gnd



![image](https://user-images.githubusercontent.com/19898602/133388891-e9a68685-f34f-4ac7-8811-79d49550fa2a.png)




In theory our idea sounds perfect, let’s code this Arduino and test our idea in real world.

The code is very simple to understand, we used the servo library, and defined basic setups and variables, the main code is such that it calculates the distance in centimeters and if the distance is less than 10 cm the servo motor performs a sweep motion to release the liquid.






Once our code is uploaded, it would be good practice to Test this project before we complete this enclosure.

in this test we can clearly see when our hand is placed above sensor and distance for ultrasonic drops below 10 cm, servo motor is engaged and alcohol hand rub is dispensed.

once the project is working properly, we can move further to next step!








Once our project seems to be working, it's time to complete the enclosure.

follow the steps to complete it:

measure the Dimensions for Ultrasonic Sensor and holes for Bottle.
make a slot for Copper wire with extra room for Moment.
mark all cutting holes.
use Sharp Blade or Drill to plot the holes.
fix everything with the help of hot glue.
And finally this project comes to life.






