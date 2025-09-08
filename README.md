# LineTrace for Micromouse with Simulink&reg;

Micromouse is a small robot about the size of your palm.
This robot can detect a black line on the floor using sensors and automatically follow the line.


## About the submission:

This submission includes two models: a simulation model and a hardware implementation model. It contains a set of .slx and .ioc files for hardware deployment, as well as an .stl file for rendering a CAD model in the simulation environment. The models are designed for student teams participating in the Micromouse competition. Teams can use this app as a reference to learn about model-based design (MBD).

![LineTracer Pic png](https://github.com/mathworks/Line-Trace-for-Micromouse/blob/main/ImageForGit/Pic.png)

## Simulation Model

1. Install the Simulink 3D Animation&trade; software and Computer Vision Toolbox&trade; software.

2. Open the LineTrace_2024b.slx model.
(Note: The files Course.stl and Tracer.stl are located in the current folder.)

3. Run the model.

![Simulation GIF](https://gitlab.com/NobuIijima/LineTracer2/-/raw/main/ImageForGit/Simulation_Gif.gif)

## Hardware Implementation Model

1. Install Embedded Coder Support Package for STMicroelectronics STM 32 Processors.
	(MATLAB&reg;, Simulink, Embedded Coder&reg;, MATLAB Coder&trade;, Simulink Coder&trade;, Embedded Coder Support Package for STMicroelectronics STM32 Processors)
2. Select the "LineTrace_Hardware" model that matches your hardware (Version 1 or Version 2) and Open the model

3. Connect your hardware to your laptop using a USB cable

4. Check the COM port number from Device Manager on your PC.

5. Update the COM port number in the Simulink model based on the value you found in step 4:
Configuration Parameters → Hardware Implementation → Target hardware resources → Connectivity → Serial port.

6.1. To perform "Monitor & Tune":
Before clicking the button, go to
Configuration Parameters → Code Generation → Build Configuration,
and set it to "Faster Runs".

6.2. To perform "Build, Deploy & Start":
Before clicking the button, go to
Configuration Parameters → Code Generation → Build Configuration,
and set it to "Faster Build".

![LineTracer Hardware GIF](https://gitlab.com/NobuIijima/LineTracer2/-/raw/main/ImageForGit/Hardware_Git.gif)

## Call to Actions
By modifying and extending each subsystem, more advanced simulations can be achieved. This model is designed as a versatile and lightweight demo, and with appropriate adaptations, it can be applied to a wide range of fields such as automotive, rockets, robotics, drones, aircraft, railways, and marine systems.

## Required Products

For Simulation:

	Simulink
	Simulink 3D Animation
	Computer Vision Toolbox

For Hardware & Support Package

	MATLAB
	Simulink
	Embedded Coder
	MATLAB Coder
	Simulink Coder
	Embedded Coder Support Package for STMicroelectronics STM32 Processors

Copyright 2025 The MathWorks, Inc.
