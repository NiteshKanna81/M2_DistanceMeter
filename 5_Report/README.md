# Distance Measurement for measuring distance using ATmega328 Microcontroller

## Introduction

The main objective of this project is to measure the distance between the object/obstacle.
In this project we are using Ultrasonics sensor. Ultrasonic Sensor sends out a sound wave signal at a frequency above the range of human hearing.
Like ultrasonic sensor there are many others, we can use a transducer to transmit a pulse and to receive the echo. The Sensor determines the distance to a target by measuring time lapses between the sending and receiving of the ultrasonic pulses.

# 4 W's an 1 H


## What

- we have made a setup based on a microcontroller in which real time distance is sensed by an ultrasonic sensor and displays measured distance on an LCD display.

## Where

- It measures accurate distance using a non-contact technology - A technology that involves no physical contact between sensor and object.

## When

- In 1959, Satomura created an ultrasonic flowmeter that used doppler technology.

## Why

- I am Developing this project for easily measure the distance between objects

## How

- By using Atmega328 an display an ultrasonic sensor mainly used to determine the distance of the target object.


# Features

## Hardware Features

- ATmega328 is commonly used in many projects and autonomous systems where a simple, low-powered, low-cost micro-controller is needed.
- A sound sensor is defined as a module that detects sound waves through its intensity and converting it to electrical signals.
- A display device is an output device for presentation of information in visual or tactile form.

## Software Features

- SimulIDE tool provides ATmega, AVR, Arduino and PIC microcontrollers that can be accessed just like other components. Features like gpsim and simavr allow you to use PIC and AVR microcontrollers, respectively.
- An automatic voltage regulator (AVR) is an electronic device that maintains a constant voltage level to electrical equipment on the same load. The AVR regulates voltage variations to deliver constant, reliable power supply.


# High Level Requirements

| ID             | Description                                                           |
| ----------------- | ------------------------------------------------------------------ |
| HLR_01 | Used to measure the distance within a wide range of 2 cm to 400 cm |
| HLR_02 | Depth of certain places like wells, pits etc can be measured since the waves can penetrate through water |
| HLR_03 | Used to avoid and detect obstacles with robots like biped robot, obstacle avoider robot, path finding robot etc. |


# Low Level Requirements

| ID             | Description                                                           |
| ----------------- | ------------------------------------------------------------------ |
|           | Power Supply :+5V DC. |
| LLR_01 | Measuring Angle: 30 degree. |                                                                                                                                       
|           | Trigger Input Pulse width: 10uS TTL pulse. |
| LLR_02 | Depth of certain places like wells, pits etc can be measured since the waves can penetrate through water. |


# SWOT ANALYSIS


## Strength:
- The distance to an obstacle can be measured with the low cost ultrasonic sensor . The sensors can measure distances form 2 to 400 cm with an accuracy of 3 mm. This sensors module includes ultrasonic transmitter, ultrasonic receiver and control circuit.

## Weakness:
- Although we fully believe in the capability of our sensors, we understand that ultrasonics are not suited for every application. Focuses of low thickness, similar to froth and fabric, have a tendency to assimilate sound liveliness. These materials may be hard to sense at long range.

## Opportunity:
- This project can be used as parking assistance systems in vehicles with high power ultrasonic transmitter. This Project can be used as burglar alarm with suitable additional software for homes and offices.

## Threats :
- Ultrasonic sensors must view a surface (particularly a hard, level surface) unequivocally (oppositely) to get adequate sound reverberation. Additionally, solid detecting requires a base target surface range, which is indicated for every sensor sort. If connection is wrong there might be chances of short-circuit.

# Bill of Materials

**Circuit** : DistMeas.simu

**Bill of Materials** :

- Hd44780-104 : Hd44780
- atmega328-105 : atmega328
- SR04-114 : SR04 
- Potentiometer-286 : Potentiometer 1 kΩ  

# Test Plan


## Obstacle Detection:
### How: Our implementation for this step requires multiple steps :
#### Step 1: Find a distance value between each pair of sensors. To test the distance
value, we may use the numbers we see for the height and length, as well as the
Pythagorean Theorem.
####Step 2: Check the angle found between each pair of sensors using the distance value
initially found.
####Step 3: Using these values, determine what each angle should approximately be to
detect different types of obstacles.
####Step 4: Detect the obstacles.


## Output: As we had steps for each test, we will again make steps for the expected outputs:
#### Step 1: Compare the outputted (through serial) value for the hypotenuse to the
Pythagorean calculated value. We expect them to be the same.
####  Step 2: Using the same technique as step 1 except calculating the angle, we should
see the same value for this calculation as well.
#### Step 3 : The values and outputs for the “obstacle detected” will be constantly
checked and rechecked to make sure the angles determine the correct obstacle.
#### Step4 : Adding Audio to the Ultrasonic Sensors.

## High level test plan
| Test ID |           Description       |      Exp I/P    |    Exp O/P   |   Actual Out  |   Type Of Test |
| --------| --------------------------- | --------------- | ------------ | ------------- | -------------- |
|  H_01   |      High accuracy     |  Choice  |    Display   |   As Expected | Scenario based |
|  H_02   | Capable of measuring a distance of up to 400 cm | Choice  |  Display    |   As Expected | Requirement Based |
|  H_03   | Measuring time lapses between the sending and receiving of the ultrasonic pulse | Choice | Display   |   As Expected | Requirement Based |

## Low level test plan
| Test ID |           Description       |      Exp I/P    |    Exp O/P   |   Actual Out  |   Type Of Test |
| --------| --------------------------- | --------------- | ------------ | ------------- | -------------- |
|  L_01   | Detection of clear objects | Choice | Display  | As Expected   | Scenario based |
|  L_02   | Provide multiple range measurements per second | Choice | Display   | As Expected  | Requirement Based |
