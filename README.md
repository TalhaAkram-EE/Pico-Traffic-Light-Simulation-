# Pico-Traffic-Light-Simulation-  
Raspberry Pi Pico Traffic Light Simulation  
Welcome to the Raspberry Pi Pico Traffic Light Simulation project! This repository contains the code and instructions to create a traffic light simulation using the Raspberry Pi Pico.   This project is ideal for beginners and enthusiasts looking to explore microcontroller programming and LED control with Arduino.  
Table of Contents  
•	Introduction  
•	Features  
•	Hardware Requirements  
•	Software Requirements  
•	Circuit Diagram  
•	Setup and Installation  
•	Code Explanation  
•	Customization  
•	Contributing  
•	License  
Introduction  
In this project, you'll learn how to simulate a traffic light system using the Raspberry Pi Pico. The setup includes three LEDs representing the red, yellow, and green lights of a   traffic signal. We'll use Arduino code to control the sequence and timing of the LEDs.  
Features  
•	Simulate a real-world traffic light system  
•	Control LEDs using GPIO pins on the Raspberry Pi Pico  
•	Easily customizable timing for each light  
•	Perfect for learning basics of microcontroller programming and LED control  
Hardware Requirements  
•	Raspberry Pi Pico  
•	Red LED  
•	Yellow LED  
•	Green LED  
•	3 x 220Ω Resistors  
•	Breadboard and jumper wires  
Software Requirements  
•	Arduino IDE  
•	Raspberry Pi Pico setup for Arduino (Follow this guide)  
Circuit Diagram  
•	Red LED: GP1 and GND  
•	Yellow LED: GP5 and GND  
•	Green LED: GP9 and GND  
Setup and Installation  
1	Install Arduino IDE:  
o	Download and install the Arduino IDE from the official website.  
2	Set up Raspberry Pi Pico for Arduino:  
o	Follow this guide to set up your Pico for Arduino development.  
3	Download the Code:  
o	Clone this repository:  
o	Or download the ZIP file and extract it.  
4	Open the Code in Arduino IDE:  
o	Launch the Arduino IDE.  
o	Open the traffic_light.ino file from the cloned repository.  
5	Upload the Code to Pico:  
o	Connect your Pico to the computer.  
o	Select the correct board and port in the Arduino IDE.  
o	Upload the code to the Pico.  
Code Explanation  
#define RED 1  
#define YELLOW 5  
#define GREEN 9  

void setup() {  
  pinMode(RED, OUTPUT);  
  pinMode(YELLOW, OUTPUT);  
  pinMode(GREEN, OUTPUT);  
}  

void loop() {  
  digitalWrite(GREEN, HIGH);  
  delay(3000);  

  digitalWrite(GREEN, LOW);  
  digitalWrite(YELLOW, HIGH);  
  delay(500);  

  digitalWrite(YELLOW, LOW);  
  digitalWrite(RED, HIGH);  
  delay(2000);  

  digitalWrite(YELLOW, HIGH);  
  delay(500);  
  digitalWrite(YELLOW, LOW);  
  digitalWrite(RED, LOW);  
}  

This code controls the sequence and timing of the LEDs, simulating a traffic light system. Modify the delay() values to adjust the duration each light stays on.  
Customization  
Feel free to adjust the timing of the lights in the code to match your desired traffic light sequence. You can also add more features, such as pedestrian signals or blinking modes.  
Contributing  
We welcome contributions! Please fork this repository, make your changes, and submit a pull request.  
Visit our website:https://poloniumtechnologies.com/  
Visit our YouTube channel:https://youtu.be/p187QXEi84U?si=t9-cfxieRt_R0vFm  
________________________________________
Enjoy building your traffic light simulation with the Raspberry Pi Pico! If you have any questions or run into issues, feel free to open an issue or reach out. Happy tinkering!
