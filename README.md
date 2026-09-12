

<img width="1280" height="640" alt="git (1)" src="https://github.com/user-attachments/assets/8920b256-2ba8-4988-b824-5351134eb4bd" />



# Home Automation 🎯


## Basic Details
### Team Name: SAKA67


### Team Members
- Team Lead: Sriyesh Kumar - Ace College of Engineering
- Member 2: Kovidh Menon - Ace College of Engineering


### Project Description
This project is an ESP32-based home automation system that allows users to control electrical appliances remotely through a mobile app.
The ESP32 communicates via Wi-Fi and controls a 2-channel relay, which switches devices such as an LED strip ON or OFF.

### The Problem (that doesn't exist)
Getting up to switch off the lights is exhausting after a long day.

### The Solution (that nobody asked for)
An ESP32-powered system that lets you switch the lights ON/OFF from your phone—because getting off the couch is overrated.

## Technical Details
### Technologies/Components Used

For Hardware:
- Main Components
1. ESP32 Development Board – Main microcontroller with built-in Wi-Fi
2. 2-Channel Relay Module – Controls two electrical loads
3. LED Strip – Used as the lighting load
4. Power Supply – Provides power to the LED strip and circuit
5. Jumper Wires – For connecting the components
6. Blynk App – Mobile interface for remotely controlling the system[List main components]
-Specifications
1. ESP32: 32-bit microcontroller, built-in Wi-Fi & Bluetooth, GPIO pins
2. Relay Module: 2 independent channels, 5V relay module
3. LED Strip: Low-voltage LED strip suitable for external DC power
4. Blynk: IoT platform for wireless device control and monitoring
5. Communication: Wi-Fi between ESP32 and Blynk
- Tools Required
1. Arduino IDE – To program the ESP32
2. Blynk IoT Platform/App – For mobile control
3. USB Cable – To program and power the ESP32
4. Jumper Wires – For circuit connections
5. Breadboard / Terminal Connectors – For assembling the circuit
6. Computer/Laptop – For coding and uploading the program

### Implementation

For Hardware:

# Schematic & Circuit
<img width="522" height="585" alt="Screenshot 2026-09-12 052136" src="https://github.com/user-attachments/assets/097521e5-ef28-4bf0-9897-f6f413f5eb78" />


Shows the physical connections between the ESP32, 2-channel relay module, LED strip, and power supply.


<img width="436" height="586" alt="Screenshot 2026-09-12 052147" src="https://github.com/user-attachments/assets/cea82ed1-0d9c-4464-963c-6445933f5cad" />


Shows the electrical working of the system, illustrating how the ESP32 controls the relay channels to switch the connected loads ON/OFF.


# Build Photos
<img width="1536" height="1536" alt="WhatsApp Image 2026-09-12 at 04 58 37" src="https://github.com/user-attachments/assets/a1f01a59-c94f-4e73-9663-5b98883d0051" /><img width="1536" height="1536" alt="WhatsApp Image 2026-09-12 at 04 58 37 (1)" src="https://github.com/user-attachments/assets/6c841fd2-85a6-4058-908f-ad0f6e18921a" />
<img width="1536" height="1536" alt="WhatsApp Image 2026-09-12 at 04 58 38" src="https://github.com/user-attachments/assets/c59895c6-ce81-4dfb-9700-06e733fdfc15" />


Components:
1. ESP32
2. led strip
3. 2-channel Relay
4. Jumper wires
5. Home automation app
6. USB cable 

   
<img width="1536" height="1536" alt="WhatsApp Image 2026-09-12 at 04 58 36" src="https://github.com/user-attachments/assets/70854fef-359a-4ca5-ad13-172c2d7bf10a" />
1. Set up the ESP32
The ESP32 was programmed to connect to a Wi-Fi network and receive control commands from the mobile application.

2. Connect the relay module
The relay's control pins were connected to GPIO pins on the ESP32. For example:

Relay VCC → appropriate supply
Relay GND → ESP32 GND
IN1 → ESP32 GPIO
IN2 → ESP32 GPIO

Each relay channel can then be switched independently.

3. Connect the loads
The LED strip and another electrical load were connected through the two relay channels. The relay acts as an electrically controlled switch, allowing the ESP32 to turn the loads ON or OFF.

4. Provide external power
A separate power supply was used for the LED/load side rather than trying to power the LED strip directly from the ESP32.

5. Develop the mobile control interface
The phone app was configured with two controls/buttons. One button sends an ON/OFF command for relay channel 1 and the other controls channel 2.

6. Program the ESP32
The code was uploaded to the ESP32 so that:

It connects to Wi-Fi.
It communicates with the home-automation platform.
It monitors the two control commands.
It changes the corresponding GPIO outputs.
The relay switches according to those outputs.

7. Test the system
The phone was used to switch the relay channels. From your video, you can see the lights turning on/off in response to the buttons in the app.



<img width="1118" height="899" alt="Screenshot 2026-09-12 051045" src="https://github.com/user-attachments/assets/06e5034c-af5f-44b7-be0f-f9e965daa8fa" />
The final build is an ESP32-based home automation system that allows electrical devices to be controlled wirelessly using a smartphone.

At the center of the system is the ESP32, which acts as the main controller. It connects to the Wi-Fi network and communicates with the mobile application. The ESP32 is connected to a 2-channel relay module, with each relay channel acting as an independent electronic switch.

The LED strip is connected to one of the relay channels. When the user presses the corresponding button in the mobile application, the command is sent through Wi-Fi to the ESP32. The ESP32 then changes the state of the appropriate GPIO pin, which activates or deactivates the relay. This switches the LED strip ON or OFF.

The second relay channel can be connected to another electrical appliance, allowing another device to be controlled independently.

The overall operation is:

Mobile App → Wi-Fi → ESP32 → 2-Channel Relay → Electrical Loads

The ESP32 and control circuitry operate on low-voltage DC power, while the relay provides switching between the controller and the connected load. The LED strip should be powered from an appropriate external power supply rather than directly from the ESP32.

Final assembled system

The finished prototype therefore consists of:

ESP32 – central controller and Wi-Fi communication
2-channel relay module – controls two independent loads
LED strip – remotely controlled lighting
External power supply – powers the LED strip/load
Jumper/connecting wires – electrical connections
Mobile application – wireless user interface

The main advantage of the final build is that the user doesn't need to manually operate the switches. The connected devices can be switched remotely from the smartphone through the ESP32.

### Project Demo

https://github.com/user-attachments/assets/4041d581-9606-46be-a4d3-19ad1a4963f8

# Video


# Additional Demos


## Team Contributions
- Sriyesh Kumar: Contributed to the hardware development of the project, including assembling the ESP32, 2-channel relay module, LED strip, and power connections. Also assisted with testing and troubleshooting the circuit.
- Kovidh Menon: Contributed to the software and IoT side of the project by programming the ESP32 and configuring the Blynk application for remote control. Also assisted with testing the communication between the mobile app and the hardware.


---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--26-26?link=https%3A%2F%2Ftinkerhub.org%2Fevents%2F1M8ORET9A1%2Fuseless-projects-3.0)



