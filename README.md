# Glove-operated-drone

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
2 Motors
2 Wheels
PI Camera
2 power supplies
LiPO Battery
  https://rogershobbycenter.com/lipoguide
Small Breadboard

Additional Notes:
Order of priority:
Drone design
Radio input
Manual Control
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


Full Project Priority Order:
=================
Build the glove and test it’s ability to transmit radio commands. 
Build the drone and program its ability to move using simple commands
Integrate glove control into the drone.
Create the remote control program 
Create control priority between client and glove


