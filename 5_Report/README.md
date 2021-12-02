# INTRODUCTION

       Nowadays, controlling the traffic becomes major issue because of rapid increase in automobiles and also because of large
       time delays between traffic lights. So, in order to rectify this problem, we will go for density based traffic lights 
       system. This project explains you how to control the traffic based on density.
       
 ## FEATURES OF TRAFFIC SIGNAL SYSTEM 
  
    In this system, we will use IR sensors to measure the traffic density. We have to arrange one IR sensor for each road;
    these sensors always sense the traffic on that particular road. All these sensors are interfaced to the microcontroller.
    Based on these sensors, controller detects the traffic and controls the traffic system.

## IDENTIFYING THE REQUIREMENTS

HARDWARE COMPONENTS:

ATmega8 controller

PCB board

IR sensors -4

LED’s-12(4-red,4-green,4-yellow)

12v Battery or adaptor

Serial cable

Connecting wires

SOFTWARE COMPONENTS:

SimulIDE

Virtual studio code

avr-gcc

Make

## SWOT ANALYSIS

STRENGTH: 

  This project helps in reducing the time delay.

WEAKNESS:

  IR sensors sometimes may absorb normal light also. As a result, traffic system works in improper way.
  
  IR sensors work only for fewer distances.
  
  We have to arrange IR sensors in accurate manner otherwise they may not detect the traffic density.

OPPORTUNITIES:

  Avoids wastage of time due to the traffic
  
  Fully automatic
  
  It provides the easy access in the traffic light
  
THREADS:

 IR sensors sometimes may absorb normal light also. As a result, traffic system works in improper way.
  
## 4W's AND 1H
 
 WHAT:
 
  This Project explains you how to control the traffic based on density.
 
 WHERE:
 
  In High traffic density areas to control traffic automatically and efficiently.
  
 WHEN:
 
  During dense traffic areas.
  High populated areas.
 
 WHY:
 
  If there will be no traffic on the other signal, one shouldn’t wait for that signal. The system will skip that signal and will move on the next one.

 HOW:
 
  It controls traffic signals automatically using sensors and microcontroller.

## HIGH LEVEL REQUIREMENTS

|ID|DESCRIPTION|STATUS|
|---|---|---|
|HLR_1|Fully Automated|Future|
|HLR_2|Sensors And Atmega328|Implemented|
|HLR_3|Alarm Interfaced with atmega328|Future|

## LOW LEVEL REQUIREMENTS

|ID|DESCRIPTION|STATUS|
|---|---|---|
|LLR_1|LEDs Interfaced with atmega|Implemented|
|LLR_2|Resistors to protect LEDs|Implemented|
|LLR_3|Cameras|Implemented|

## DESIGN
## Behavioral Diagram 1
![Behavioral Diagram](https://user-images.githubusercontent.com/89175883/143678567-ae6b864c-503f-49a2-8790-d0c495754d55.jpg)

## Behavioral Diagram 2
![Behavioral Diagram 2](https://user-images.githubusercontent.com/89175883/143685127-ca11e48f-0f3b-4469-8e56-b6c6211e22bb.jpg)

## Structural Diagram 1
![structural Diagram 1](https://user-images.githubusercontent.com/89175883/143678490-fa3aa0b3-1b33-4676-917d-0d2f3a59e0e4.jpg)

## Structural Diagram 2
![structural Diagram 2](https://user-images.githubusercontent.com/89175883/143846020-541b4416-aa81-45b4-81c5-75538766b749.jpg)

## Block Diagram of density Based Traffic Signal System
![Block-diagram-of-a-density-based-traffic-control-system](https://user-images.githubusercontent.com/89175883/143678740-09661206-175e-4652-ad2d-39b0fb06b8cd.png)

## Simulation Image
![Circuit Simulation](https://user-images.githubusercontent.com/89175883/144375630-e623e24b-22c4-4759-a6a1-b08b7eccf356.jpeg)

## HIGH LEVEL TESTING SCENARIOS

|ID NO|DESCRIPTION|EXPECTED I/P|EXPECTED O/P|ACTUAL O/P|TYPES OF TEST|
|---|---|---|---|---|---|
|H_01|Check and verify whether the traffic light led's are working or not|---|Led's should be displayed|Led's should be displayed|Requirement Based|
|H_02|Check and verify whether the traffic light is working for that particular time|---|Light should be working at that particular time|Light should be working at that particular time|Scenario Based|
|H_03|Check and verify whether the signal is skipped when there is no traffic on that road|---|Signal shouls be skipped|Signal should be skipped|Boundary Based|

## LOW LEVEL TESTING SCENARIOS

|ID NO|DESCRIPTION|EXPECTED I/P|EXPECTED O/P|ACTUAL O/P|TYPES OF TEST|
|---|---|---|---|---|---|
|L_01|If you receive logic 0 from any of these sensors, we have to give the green signal to that particular path and give red signal to all other paths|---|It works|It works|Requirement Based|
|L_02|Check whether the sensors are working properly during rainy days or not|---|Sensors should work|sensors should work|Scenario Based|
|L_03|Check whether the light vehicles are sense by the sensor or not|---|Sensor detected|Sensor Detected|Boundary Based|
