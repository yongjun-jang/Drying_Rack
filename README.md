Smart Drying Rack System IoT & MCU Based Automatic Laundry Drying System

Overview This project presents a smart drying rack system designed to
improve laundry drying efficiency using an embedded control system. The
system monitors environmental conditions and automatically controls a
fan and drying mode to accelerate the drying process. The project was
developed as part of a university engineering competition using an
ATmega328P microcontroller.

System Architecture The system consists of the following components: -
ATmega328P Microcontroller - Environmental sensing via ADC inputs - Fan
motor control using PWM - LCD display for system status - User
interaction via external interrupts - Power control using MOSFET
switching

Key Features Automatic Drying Mode The system analyzes sensor input
values and automatically determines whether additional airflow is
required.

PWM Fan Speed Control Fan speed is controlled using PWM signals,
allowing adjustable airflow intensity depending on drying conditions.

Interrupt-Based User Input External interrupt signals allow users to
change operation modes without interrupting the system loop.

LCD Monitoring The system provides real-time information including
current drying mode, system status, and sensor values.

Hardware Design The circuit was designed using KiCad and includes: -
ATmega328P microcontroller - MOSFET-based fan control - LCD interface -
ADC sensor input circuit - interrupt switch interface

Firmware Architecture Main components: - main.c : Main system control
loop - adc.c / adc.h : Sensor data acquisition - pwm.c / pwm.h : Fan
speed control - timer.c / timer.h : Timer-based scheduling -
external_interrupt.c : Mode control - lcd.c / lcd.h : LCD display
interface - gpio.c / gpio.h : I/O control - usart.c / usart.h : Serial
communication - mode.c / mode.h : Drying mode logic

Development Environment Microcontroller: ATmega328P Programming
Language: C Tools: Atmel Studio, KiCad

Project Results The system demonstrates automated drying airflow
control, stable MCU-based embedded operation, and modular firmware
architecture.

My Contribution - Embedded firmware development (C) - PWM fan control
implementation - ADC-based sensor data acquisition - Interrupt-driven
mode control - System integration and debugging

Repository Structure Drying_Rack 
Drying_Rack
│
├─ firmware
│   ├─ main.c
│   ├─ adc.c
│   ├─ pwm.c
│   ├─ timer.c
│   ├─ lcd.c
│   └─ external_interrupt.c
│
├─ hardware
│   └─ atmega328p.kicad_sch
│
└─ documentation
    └─ project_poster

Future Improvements - IoT connectivity for remote monitoring -
humidity-based drying control - machine learning-based drying
prediction - mobile application integration
