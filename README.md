# Object_Avoidance_Robot
## ABSTRACT
This project presents an obstacle avoidance car using ESP8266 microcontroller, designed to detect the obstacles and steers clear of them. The obstacles can be detected using an ultrasonic sensor by sending an ultrasonic wave and receiving them. Then the distance of the obstacle can be calculated by the distance formula. Then an alert message will be sent to the mobile phone of the person who is controlling the car through telegram.

The direction and speed of the car can be controlled by the controlling device which is having an application ESP8266 WIFI ROBOT CAR.  A relay is used to reduce power consumption, because the motors will consume more power to work. Additionally, the device is IOT-enabled, allowing users to monitor and control the working process through BLYNK IOT INTERFACE application. This is efficient, low cost device allowing to avoid the obstacles.
____

## Features

**1.Obstacle Detection and Avoidance:**

 - Uses an ultrasonic sensor to detect obstacles in the path.
 - Calculates distance using time-of-flight of ultrasonic waves.
 - Automatically steers clear of obstacles.

**2.ESP8266 Microcontroller Integration:**

  - Central control unit for handling sensor inputs, decision-making, and communication.
    
**3.Mobile Alert System:**
    
  - Sends obstacle alerts via Telegram to the user’s mobile phone.

**4.Wireless Control:**

  - Direction and speed of the car can be controlled through the ESP8266 WiFi Robot Car App.
    
**5.Relay-Based Power Management:**
  - A relay is used to optimize power consumption, particularly for high-power motor operation.

**6.IoT Monitoring via Blynk:**

  - Real-time status monitoring and control via Blynk IoT Interface.
  - Remote access to car functions from anywhere.
______
## Work Flow
**1.Power ON and Initialization:**

+ When the system is powered on, the ESP8266 microcontroller initializes all modules: ultrasonic sensor, relay, motor drivers, and Wi-Fi connection.

+ It also connects to the Blynk IoT platform for remote control and monitoring.

**2.Ultrasonic Obstacle Detection:**
+ The ultrasonic sensor continuously emits sound waves.
+ When the wave hits an obstacle, it reflects back to the sensor.

 + The sensor calculates the distance using the formula: 
   ### Distance = (Time x Speed of Sound) / 2

**3.Decision-Making (Avoidance Logic):**

+ If the distance measured is less than a set threshold, the ESP8266 decides an alternate path.

+ It sends signals to the motor driver circuit to:

   - Stop

   - Turn left or right

   - Or reverse, depending on the obstacle location.

**4.Motor Control and Power Management:**

+ A relay module is used to manage power supply to the motors.

+ This ensures the motors only draw power when needed, reducing energy consumption.

**5.Wireless Control and Monitoring:**

+ The user can manually control direction and speed through the ESP8266 WiFi Robot Car App.

+ The car sends real-time data to the Blynk IoT Interface, allowing the user to:

    + Monitor obstacle distance

    + View system status

    + Remotely control movement

**6.Telegram Alerts:**

+ If an obstacle is detected, the ESP8266 sends an alert message via Telegram to the user's mobile.

+ This improves situational awareness even when the user isn’t actively monitoring the app.

**7.Continuous Operation:**

+ The system loops through sensor readings and control logic continuously.

+ It adjusts movement dynamically based on obstacle presence and user input.

_____
## Advantages:
**1.Cost-Effective:**

- Uses low-cost components while providing smart automation features.

**2.Efficient and Power-Saving:**

- Employs a relay mechanism to reduce unnecessary power drain from motors.

**3.Enhanced Safety:**

- Obstacle detection helps prevent collisions and potential damage.

**4.User-Friendly Operation:**

- Easy control using mobile apps with intuitive interfaces.

**5.Remote Monitoring and Alerts:**

- Provides live updates and notifications via Telegram and Blynk, enhancing user awareness and control.

**6.IoT-Enabled Smart System:**

- Combines automation, control, and communication in a single compact system.
____
# Getting Ready

+ Install necessary libraries in arduino IDE.
+ Install the ESP8266 WiFi Robot Car Application and connect it to the ESP using Blutooth.
