# **The CNC pen plotter**

This project aims to create a Cartesian robot with a closed-loop control system for MCT333 ASU course , including actuator sizing, electrical schematic design and software framework. The robot has an overhead structure controlling horizontal motion and a robotic arm for vertical motion with a pen effector.
## **Table of Contents**

- [Abstract](#Abstract)
- [Introduction_to_Cartesian_Robot](#Introduction_to_Cartesian-Robot)
- [Flowchart_open_loop](#Flowchart_open_loop)
- [CAD_Detailed_Design(OpenLoop)](#CAD_Detailed_Design(OpenLoop))
- [MATLAB_Model_and_Simulation(OpenLoop)](#MATLAB_Model_and_Simulation(OpenLoop))
- [Electrical_Schematic_and_Simulation(OpenLoop)](#Electrical_Schematic_and_Simulation(OpenLoop))
- [Trials(OpenLoop)](#Trials(OpenLoop))
- ....................................
- [Flowchart_closed_loop](#Flowchart_closed_loop)
- [CAD_Detailed_Design(closedloop)](#CAD_Detailed_Design(closedLoop))
- [MATLAB_Model_and_Simulation(closedLoop)](#MATLAB_Model_and_Simulation(closedLoop))
- [Electrical_Schematic_and_Simulation(closedoop)](#Electrical_Schematic_and_Simulation(closedLoop))
- [Component_selection](#Component_selection)
- [Trials(closedLoop)](#Trials(closedLoop))
- [Software_Design_and_Framework](#Software_Design_and_Framework)

## **Abstract**

CNC (Computer Numerically Controlled) devices are widely used in various types of devices such as plotters, vinyl cutters, 3D printers, milling machines, and others. This paper aims to present a detailed design and simulation of a cartesian robot with a closed-loop control system. The cartesian robot has an overhead structure that controls the motion in the horizontal plane and a robotic arm that actuates motion vertically. The robotic arm has an effector or machine tool attached to the end of the arm, which is a pen. The design and simulation are performed using various software such as CAD software, MATLAB, and Simulink. The actuator sizing is calculated using Simulink, and the electrical schematic is designed and simulated using software. The component selection, software design and framework, and trials are also discussed in detail.

## **Introduction_to_Cartesian_Robot**
Cartesian coordinate geometry is an excellent method for mapping three-dimensional space in a simple, easy-to-understand numerical system. In the Cartesian system for three-dimensional space, there are three coordinate axes that are perpendicular to each other (orthogonal axes) and meet at the origin. The three axes are generally referred to as the x-axis, y-axis, and z-axis. Any point in three-dimensional space is represented by three numbers as (x, y, z). X represents the distance of the point from the origin along the x-axis, y is the distance from the origin along the y-axis, and z is the distance from the origin along the z-axis.

Cartesian robots have an overhead structure that controls the motion in the horizontal plane and a robotic arm that actuates motion vertically. They can be designed to move in x-y axes or x-y-z axes. The robotic arm is placed on the scaffolding and can be moved in the horizontal plane. The robotic arm has an effector or machine tool attached to the end of the arm, which is a pen.

# **For Open Loop System**
### **Flowchart_open_loop**
![For Open Loop System](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Flowchart%20for%20open%20loop.png "For Open Loop System")

### **CAD_Detailed_Design(OpenLoop)**
![CAD_Detailed_Design(OpenLoop)](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Cad%20detailed%20Design%201.png "CAD_Detailed_Design(OpenLoop)")

![CAD_Detailed_Design(OpenLoop)](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Assembly%202.png "CAD_Detailed_Design(OpenLoop)")

### **MATLAB_Model_and_Simulation(OpenLoop)**

![MATLAB_Model_and_Simulation(OpenLoop)](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/MATLAB%20model%20and%20simulation.png "MATLAB_Model_and_Simulation(OpenLoop)")

![MATLAB_Model_and_Simulation(OpenLoop)](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/MATLAB%20model%20and%20simulation%202.png "MATLAB_Model_and_Simulation(OpenLoop)")

![MATLAB_Model_and_Simulation(OpenLoop)](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/MATLAB%20model%20and%20simulation%202.png "MATLAB_Model_and_Simulation(OpenLoop)")

![block diagram of Simulink](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/block%20diagram%20of%20Simulink.png "block diagram of Simulink")

![blocks for PID-control](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/blocks%20for%20%20PID-control.png "blocks for PID-control")

![simulation](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/simulation.jpg "simulation")


### **Electrical_Schematic_and_Simulation(OpenLoop)**

![Electrical schematic and simulation](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Simulation%201.jpg "Electrical schematic and simulation")

![Simulation 1](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Electrical%20schematic%20and%20simulation.jpg "Simulation 1")


![Simulation 2](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Simulation%202.jpg "Simulation 2")


### **Trials(OpenLoop)**

# **For closed Loop System**
A closed loop control system is a mechanical or electronic device that automatically regulates a system to maintain a desired state or set point without human interaction.
![closed loop](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/closed%20loop%20control%20system.png "closed loop")

### **Flowchart_closed_loop**
in closed loop we will control dc motors using PID and encoders, so we will use only Inkscape to get GCODE from, and universal G-code sender to send to Arduino. then we code Arduino file and make it reads the new position of each axis from this G-code file, then calculate the number of Rotation needed to be rotated by each axis from this equation (x_new-x_pre )×(number of rotation /mm)

![For Open Loop System](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/Flowchart%20for%20closed%20loop.png "For Open Loop System")

### **CAD_Detailed_Design(closedLoop)**
### **MATLAB_Model_and_Simulation(closedLoop)**
### **Electrical_Schematic_and_Simulation(closedLoop)**
### **Component_selection**
- GT2 Bore 5mm 20 Teeth Timing Aluminum Pulley Fit GT2-6mm Open Timing Belt
- Meters GT2-6mm Open Timing Belt
- DC Geared Motor 50r/min , 0.62 N.m 2.9 Watt
- C-Beam Linear Rail
- 3d printing parts
- Servo motor
- Metal V-Groove Bearing Kit
- DC motor shield
- Arduino Mega
- Arduino UNO
- Rotary Encoder E6B2-CWZ3E (1000 P/R)
- Power supply 12v - 5A


### **Trials(closedLoop)**


### **Software_Design_and_Framework**
- **Inkscape** 
it’s our HMI. used to convert the image needed to be drawn into path and then creates GCODE file to be sent to Arduino.
![SW](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/is.jpg "SW")

- **Universal G-code sender (UGS)**
it’s the communication between our machine and computer, it has advantages of like more oversight of the machine and a real time view of the toolpath.  
![SW](https://github.com/Esmtra/The_CNC_pen_plotter/blob/main/Img/ugs.png "SW")

- **GRBL**
it’s the main software running on Arduino that converts G-code into electrical signals to motor drivers (CNC shield). 
Run GRBL on Arduino:
download the GRBL library and extract it in the Arduino's library folder. now open Arduino ide and open GRBLMAIN in example sketches, and upload "GRBL to Arduino Sketch" to your Arduino UNO board. and that's it. you have uploaded GRBL to your Arduino board

- **GRBL-Plotter**
GRBL-Plotter is a graphic converter and gcode sender for all purposes.
The main focus is on the post-processing of vector graphics, the specialty is the preparation of the generated Gcode, which is based on properties of the imported graphics, such as Layer, pen color or pen thickness




## **Contact**

- **[Eslam S Rady](mailto:Eselmtrawy@gmail.com)** - Email address
- **[GitHub](https://github.com/Esmtra)**     - GitHub profile link
- **[LinkedIn](https://www.linkedin.com/in/eslam-mtra-1714201b7/)**    - LinkedIn profile link
