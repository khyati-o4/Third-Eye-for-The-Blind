# Object-detection using opencv

# Objective

In this project, we want to build a wearable third eye for the blind that runs on Arduino. The "Third Eye for Blind" is a device that uses sound and touch to assist the blind compensate for their lack of vision. In order to alert the user of an impending obstacle, it combines audio and vibration signals.
There are no products like this one on the market that are so cheap and straightforward, and that can be worn like a garment. It will significantly help the community when implemented on a big scale and with enhancements to the prototype.

# About the Project

The eyes are an essential component of the human body, making blindness a terrible disease for those who experience it. For those who are blind or visually impaired, there are a variety of tools and smart technologies that can be used for navigating, but most of them are not very portable and require a lot of training to use. Designing an item that will be especially helpful to persons who are physically disadvantaged and frequently depend on others is the aim of this project, Third Eye for the Blind. 
By sensing surrounding obstacles with the aid of a wearable band that generates ultrasonic waves and alerts users with a buzzing sound or vibrations, the third eye for Blind job is a breakthrough that enables outwardly impaired persons to move around and between different regions with speed and assurance. By pointing out the obstacles, it enables the client to walk freely even if they appear to be hindered. They only need to attach this device to their bodies as a band or piece of fabric.
In this device, an Ultrasonic module and a Microcontroller are used to determine the location of the snag. The predicted snag distance is communicated to the outwardly hindered person as a ringer and vibrations. Using this, the person can move in different directions and avoid collisions. The final products of the work will be gloves with a wearable band attached to the gloves to which every segment is connected on a PCB, and which operate with an extremely high level of precision and unwavering quality.

# Components required

• Arduino UNO  
• ESP 32 cam module\
• HC-SR04 Ultrasonic sensor\
• Vibrating Motor\
• Buzzer\
• LED RGB\
• Connecting wires\
• Jumper wires\
• Breadboard/Perf board

# Working

![working](https://user-images.githubusercontent.com/77969198/175667053-7d0a8bf3-f1fa-484d-987c-d85c2780e679.png)

Arduino UNO is being programmed with ESP-32 Cam module (programmed using python OpenCV), HC-SR04 ultrasonic sensor, vibrating motor, RGB LED, and buzzer. At the end, after all the connections are done to the Arduino board upload the code to Arduino board and power the other modules using a power bank or the power supply. The Ultrasonic sensor here used as a transceiver. The ultrasonic waves are emitted by the transmitter when the objects are detected. Both the transmitter and receiver re resent inside the ultrasonic sensor.

When the ultrasonic sensor detects the wave impulses from the obstacle near it, the cam module will scan the image and capture it in frames and it will give out the output in form of sound (in the form of speech on obstacle/object recognition), vibration (through vibrating motor) and light (LED RGB). As the blind man is in the proximity of the obstacle, the RGB LED will change from green (safer distance) to blue and when the obstacle is to the nearest, the RGB LED will turn red. The same goes for the buzzer and vibrating motor which will increase the intensity as the object comes closer to the man.

A. Module 1- Arduino UNO

B. Module 2-Buzzer Mode
When the obstacle comes in front of the device it will produce a beep sound and if the way is clear then no sound will be produced.

C. Module 3- Vibration mode
Vibration along with the beep sound will be felt by the device wearer whenever the obstacle is nearer which will help to navigate in a better way.

D. Module 4- ultrasonic sensor
The Ultrasonic sensor is interfaced accordingly. The Ultrasonic sensor pin VCC is connected to the Arduino pin VCC, the Ultrasonic sensor pin GND is connected to the Arduino pin GND, Ultrasonic sensor pin Trig is attached to the Arduino pin 12, Ultrasonic sensor pin Echo is connected to the Arduino PIN 12. The switch used here is for selecting the mode. (Buzzer or vibration mode.)

E. Module 5- RGB led
The RGB LED will change from green (safer distance) to blue and when the obstacle is to the nearest, the RGB LED will turn red.

# Software Implementation

![tinkercad](https://user-images.githubusercontent.com/77969198/175667100-71fed583-abe6-4894-a07d-0d152c2201da.png)

Link for Tinkercad Simulation:

https://www.tinkercad.com/things/0RYi3WyU3Gi-copy-of-ultrasonic-sensor-with-rgb-2/editel?sharecode=HzsCMdp43oRKJ7j1CZskVqlnSpl86troYn2ihZs95MA

OpenCV is then used for object detection and localization through a small camera fitted in the ESP-32 Cam module system. And the text-to-speech library will convert the output to speech which the blind can hear. The class id will be first detected and its reference class name, this will feed the input to the text-to-speech module of python which converts it into audio.

# Results and Discussion

Snaps of object detection

![snap1](https://user-images.githubusercontent.com/77969198/175667141-7634105d-b4a4-4e5b-84d6-fb985a5ea8c3.png)

![snap2](https://user-images.githubusercontent.com/77969198/175667176-a6697d47-2712-46b5-b840-03157bfe7c88.png)

Hardware circuit demonstration

![circuit](https://user-images.githubusercontent.com/77969198/175666162-b4dd3cb9-cd85-4472-ab5f-cfe98e477990.jpeg)

![circuit2](https://user-images.githubusercontent.com/77969198/175666289-595a002e-60ce-4c4a-8748-4b79b5d793ea.jpeg)


# Drive link for working demonstration

https://drive.google.com/drive/folders/1glxZaLZ4dd54n-nVrS-1DmfNCz7_vgPH?usp=sharing

# Conclusion

This project provided the design and architecture for a novel Virtual Eye for the Blind based on Arduino that can identify objects and obstacles in front of users and provide warning signs in the form of audio messages and vibrations. An electronic guidance system that is straightforward, affordable, effective, portable, adjustable, and user-friendly is suggested in order to give the blind and visually impaired with helpful aid and support. The system's ability to pinpoint the origin and distance of potential hazards for the blind makes it unique and effective. It has the ability to detect and scan for obstacles. The blind will be able to go from one area to another if the planned architecture is designed correctly.

