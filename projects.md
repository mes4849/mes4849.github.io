---
title: Projects
layout: default
---

## Real-Time Flight Software | Texas A&M CanSat
### *Lead Developer*
<a></a>
### About this Project
This project is part of my work for Texas A&M's CanSat team. We participate in the annual [CanSat competition](http://www.cansatcompetition.com/) - with a unique objective every year, our team is constantly learning new skills and working to implement new functionality.

The FSW is developed in a highly structured, modular way such that functionality can easily be added or removed as the project needs. We make use of OOP, interrupt routines, and serial I/O. The FSW is written purely in C++, except for hardware libraries, and modified header files which are sometimes in C.

### Project Specifics
While specific requirements for our FSW change year to year, we employ as much code reusability as possible and use components that have existing development to support our operations
-   **Host**: Atmel 8-bit AVR Chip - Bare Metals Programming  
    Our FSW is easily adaptable to other MCUs, especially ones which can operate with the Arduino standard libraries.
-   **Development**: C/C++ with strong use of Arduino standard libraries (Serial, Software Serial)  
    This allows us to make our code as platform agnostic as possible
-   **Features**: Byte Addressing for hardware abstraction & communication ; I2C and Serial communication ; Interupt Routines ; flight state  
-   **Peripherals**
    -   IMU (currently 6-axis InvenSense MPU 6050 with DMP)
        - yaw, pitch, roll ; correpsonding rates
        - x,y,z acceleration & gravity vector
    -   Barometer (currently BMP 280 * 2)
    -   GPS (currently built around the MTK3339 chipset)
    -   Blade Spin Rate sensor (photointerruptor w/ custom op-amp circuit and algorithm)   
    
<br>

## Algorithmic Trading | Personal
<a></a>
### About this Project
I love following financial markets and trading securities. With the advent of no-comission trading platforms, especially ones like [Alpaca](https://alpaca.markets/) which are aimed specifically at algorithmic trading, it has become easier than ever to get take part of something that has historically been dominated by HFT and big institutions.

My application makes use of concurrency, OOP, exception handling, REST API(s), Streaming API(s) (websockets), and of course, statistical analysis for financial applications. Without getting into details, my strategy focuses on intra-day, high volume trading with a focus on swing points for short outlook movements.

### Project Specifics
-   **Host**: My application works on any properly configured Python environment, but due to the resources and networking requirements, it runs on a dedicated AWS instance. 
-   **Development**: All development has been done in Python, but I plan on porting it over to C# since the program workflow and required libraries exist in both ecosystems.
-   **Features**: Terminal application with real-time logging to text file and console ; User input for *start/stop* operations, *asset dumping*, statistical data *P/L(day) , Open Positions*