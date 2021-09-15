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

![image](https://user-images.githubusercontent.com/19898602/133388891-e9a68685-f34f-4ac7-8811-79d49550fa2a.png)
![image](https://user-images.githubusercontent.com/19898602/133389115-46bb4f12-60a5-4953-8924-afa54f1d8c03.png)


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

I have made this project on Zero PCB but if you are planing for ant custom PCB there is good new for you.

Yes PCB are the heart of the electronics based project usually we hesitate to try custom PCB and opt to homemade solutions

like breadboard or Zero PCB earlier I also was in the same boat, I hesitate to try custom PCB my belief was they are much expensive.

but then I came to know about [JLCPCB.com](https://jlcpcb.com/IAT) and I was totally surprised how low price PCB's are they offering 

there PCB quality is best in market, now I always go with PCB for my project and [JLCPCB.com](https://jlcpcb.com/IAT) is my trusted 

PCB manufacturer, you can also try there PCB service for more details you can visit their website [JLCPCB.com](https://jlcpcb.com/IAT)



![image](https://user-images.githubusercontent.com/19898602/130722559-0080ae28-08c6-4ad1-9522-e8571cfabbef.png) ![image](https://user-images.githubusercontent.com/19898602/130722577-c30b7b43-ea89-4847-9c6b-058f9fabeda3.png)


![image](https://user-images.githubusercontent.com/19898602/130722585-b5268db1-5f17-428f-ba60-b823140f2a70.png)



![image](https://user-images.githubusercontent.com/19898602/133389322-62c6d59b-27bc-4443-96f4-80f1710d8873.png)
![image](https://user-images.githubusercontent.com/19898602/133389357-139ce620-8563-467d-b5ca-b39bc0cd2807.png)



In theory our idea sounds perfect, let’s code this Arduino and test our idea in real world.

The code is very simple to understand, we used the servo library, and defined basic setups and variables, the main code is such that it calculates the distance in centimeters and if the distance is less than 10 cm the servo motor performs a sweep motion to release the liquid.


![image](https://user-images.githubusercontent.com/19898602/133389464-9a918b5d-5f56-427b-a4ec-1ce670335e18.png)
![image](https://user-images.githubusercontent.com/19898602/133389501-1f51aef5-473b-4826-8272-e34089ef94c0.png)






Once our code is uploaded, it would be good practice to Test this project before we complete this enclosure.

in this test we can clearly see when our hand is placed above sensor and distance for ultrasonic drops below 10 cm, servo motor is engaged and alcohol hand rub is dispensed.

once the project is working properly, we can move further to next step!

![image](https://user-images.githubusercontent.com/19898602/133389567-599e7c4c-dfe9-4a00-8604-06bf59881173.png)
![image](https://user-images.githubusercontent.com/19898602/133389601-0ee73aef-1e6a-479d-bf57-8c1046b925b6.png)




Once our project seems to be working, it's time to complete the enclosure.

follow the steps to complete it:

measure the Dimensions for Ultrasonic Sensor and holes for Bottle.
make a slot for Copper wire with extra room for Moment.
mark all cutting holes.
use Sharp Blade or Drill to plot the holes.
fix everything with the help of hot glue.
And finally this project comes to life.


![MVI_0001_3_2](https://user-images.githubusercontent.com/19898602/133389811-cc325561-def2-41ab-8b66-bcbd209a71a8.gif)




