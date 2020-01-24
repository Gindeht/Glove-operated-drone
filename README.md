# Glove-operated-drone

Table of Contents:
Glove Component:
  Overview:
  Parts List:
  Additional Notes:
Drone Component:
  Overview:
  Parts List:
  Additional Notes:
Client Component:
  Overview:
  Parts List:
  Additional Notes:
Full Parts List:
Full Project Priority Order:
Drone Component Details:

Glove Component:
=================
Overview: 
The glove itself is designed to be a general purpose wireless controller using a 433 MHz radio transmitter. The drone is being constructed to be compatible with this glove. The glove itself will be run by an Arduino Nano Every and will feature analog input from all 5 fingers, analog joystick control, 3 total button inputs, an LED for simple status communication, and a decent range for controlling a receiving device.

Parts List:
Arduino Nano Every
5 Flex Sensors
Joystick (with shaft button)
2 Stand-Alone Buttons
RGB LED
433 MHz Transmitter
Welding Glove
5V Power Supply

Additional Notes:
Order of Priority:
Build the glove
Test basic hardware functionality
Integration with drone component

Drone Component:
=================
Overview:
We’re going to handbuild our drone. This is because we have very specific needs regarding the amount of weight and stability the drone will need to lift/have. Again we are going to use a Raspberry Pi 4 to handle flight commands and other things. We will have one camera mounted on the drone as well as radio input and camera output. The drone itself is controllable from a software client as well has the glove component. An additional goal is to have an ultrasound/laser rangefinder package attached to the drone to help with making a 3D model of its surroundings. This last part is an extra thing we should only work on if we have time, we should attach the ultrasound sensors and laser rangefinder so we can use them. 

Parts List:
Raspberry Pi 4
4 Motors
4 Props
PI Camera
2 power supplies
LiPO Battery
  https://rogershobbycenter.com/lipoguide
Small Breadboard

Additional Notes:
Order of priority:
Drone design
Simple 4 rotor design, need 2 power supplies
Try to get the drone to be completely balanced so we don’t need to account for that inflight
Radio input
Flight (manual control)
Integration with glove
Camera output
Full integration with client
3D Model building/pathfinding

Client Component:
=================

Overview:
The drone outputs video feed from the camera and receives flight commands via radio waves. We are going to use the output of the drone to build a program that can control the drone with a camera feed. We will be using a normal Raspberry PI for this component. A small LCD screen will be used to display the camera feed. Because of the nature of the drones input, we need to use a PI because normal desktop computers do not have radio compatibility. 
Parts List:
Raspberry PI 4
LCD Screen
Keyboard
Mouse
Radio transmitter

Additional Notes:
Order of priority:
Radio transmit 
Camera input to screen output
Full control over the drone
Establish priority of control with glove. 

Full Parts List:
=================
<will copypaste when we complete all sections, we will need to add links to buy them if we can as well as cross out the things we already have. >
.

Full Project Priority Order:
=================
Build the glove and test it’s ability to transmit radio commands. 
Build the drone and program its ability to fly using simple commands
Integrate glove control into the drone.
Create the remote control program 
Create control priority between client and glove

Drone Component Details:
=================
Design: Standard 4 motor design 
Drone parts:
https://www.instructables.com/id/The-Drone-Pi/
https://www.zdnet.com/article/how-to-build-a-200-smart-drone-with-the-pi-zero/
alibaba
Streaming PiCam to another PC using Python Sockets
https://www.youtube.com/watch?v=bWwZF_zVf00
PI Starter Kit
https://www.amazon.com/CanaKit-Raspberry-4GB-Starter-Kit/dp/B07V4G63M1?th=1
Connection between Pis
There is an option to setup the Pi aboard the drone as an access point, to where any PC that connects to it (like a wifi router) can receive and transmit commands/messages using wireless “internet”. 
Ad hoc
https://spin.atomicobject.com/2013/04/22/raspberry-pi-wireless-communication/
Gyroscope sensor:
https://www.amazon.com/SunFounder-MPU6050-Raspberry-Gyroscope-Accelerator/dp/B0151GI5VI
Drone esc replacement?
https://www.raspberrypi.org/forums/viewtopic.php?p=347830#p347830
Pigpio?
https://www.instructables.com/id/Driving-an-ESCBrushless-Motor-Using-Raspberry-Pi/

Planned Schedule:
=================
Get the PI 4 Starter kit, motor controller, and motors
Test motor functionality and programmability
Build the drone frame and mount the PI/MC as well as rotors
Test dual power supply
Test hover capabilities
Test radio functionality/ad hoc
 
