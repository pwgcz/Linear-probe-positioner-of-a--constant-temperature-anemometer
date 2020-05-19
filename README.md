# Linear probe positioner of a constant temperature anemometer
## Overwiev
The aim of the work was to design and construct a linear probe positioner with a constant temperature anemometer for automatic positioning of the Dantec Dynamics 55P6 probe
to measure velocity profile of of the stream flow.
The device assumed positioning the probe in one axis inside the most popular sizes of pipelines used in the Flow Laboratory.
The scope of work included writing a device control panel in the LabView program,
designing a dedicated PCB to communicate with the control panel and position control,
writing a C language program that integrates most of the device components, and
designing a device that meets the design requirements.

## Purpose
Knowledge of the actual velocity profile is applicable in flow metrology. It allows
validation of speed profiles obtained by numerical calculations, or assumed in a
theoretical manner. This allows for more accurate design of pipeline networks used to
measure stream flow, with the requirements set.

## Device
### Overwiev
The device consists of a steel ring into which a sleeve is screwed. Inside it is a probe
with a stepper motor. The engine connects to the ring with bent sheets. Universal
assembly is ensured by replacing the ring and the bent sheet. The positioner is
controlled and monitored using a computer with the LabView program installed.

### Requirements
The design of the device assumed assembly between standard flanges according
to EN 1092-1: 2013, protection of the probe against damage during positioning and its
replacement, ensuring a constant axial position of the probe during movement,
positioning resolution less than 0.5 mm and installation on DN50, DN65, DN80 and
DN100. All set requirements have been met.

#### Model
<img width="135" alt="probe" src="https://user-images.githubusercontent.com/62465226/82311448-01bd9f00-99c6-11ea-9e43-6b0d6343a7cb.png">


#### installed device
![IMG_20200117_160717](https://user-images.githubusercontent.com/62465226/82312961-05eabc00-99c8-11ea-910b-06c2b8f5bb1c.jpg)
## Hardware
Core of the system is  dedicated PCB designed by myself. I use STM32 F103RB microcontroller. Function of microcontroller was 
to communicate between LabVie program using UART and control step motor by setting given position from user and retrive actuall position.
## Software
Code for microcontroller is stored in this repository.







