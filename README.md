# Macondo-Drone
Repository containing all the information &amp; hardware files for my Macondo hackathon project.

Project Motivation
Inspired by competitive drone racing videos and Raffaello D'Andrea's TED Talk on quadcopter dynamics, this project bridges theoretical aeronautics with hands-on robotics. By applying prior experience in CAD and electronics, the objective is to design, source, and assemble a fully functional, high-performance First-Person-View (FPV) drone from scratch.

Research & Feasibility
Initial research focused on flight physics, propulsion dynamics ($5\times4\times3$ propeller sizing), and electronic subsystem compatibility
Power & Processing: Selected a combined Flight Controller (FC) and Electronic Speed Controller (ESC) stack to manage sensor processing and high-current motor output, paired with high-discharge 6S Li-Po batteries for optimal thrust-to-weight ratio.
Video Transmission: Evaluated digital versus analog systems, opting for analog due to its minimal latency, wide compatibility, and cost efficiency.Structural
Design: Modeled a custom frame in Onshape CAD and printed test parts in PETG at a university design lab. Thermal and stress evaluation showed PETG's limitations near hot soldering joints, leading to a final selection of a 225mm carbon fiber frame for crash durability.

Bill of Materials (BOM)
Flight Stack: DolphinRC 60A ESC + F405 FCMotors & Props: MEPS Neon 2207 2050KV motors (x4) with HQProp E-thix S5 propellers
Video System: SpeedyBee TX800 VTX paired with a Caddx Ratel 2 cameraRadio Link: SoloGood ELRS receiverFrame: PHISITAL Mark5 DC/X O3 225mm Carbon Fiber frame
Power & Tools: Ovonic 6S 1300mAh batteries (x2) and a NewBeeDrone practice soldering kit

Total Estimated Budget: £286.72 (~$387.27 USD)

Assembly & Implementation Plan
Soldering Preparation: Practice wire tinning and pad connections on the practice kit before soldering motor leads, XT60 power connections, and a noise-filtering capacitor to the ESC.
Stack & Frame Assembly: Mount the motors to the carbon fiber arms and soft-mount the FC/ESC stack using rubber grommets to isolate gyro sensors from motor vibration.
Peripherals Integration: Wire the Caddx camera, SpeedyBee VTX, and SoloGood ELRS receiver to their designated FC UART pads.
Software Configuration: Flash Betaflight firmware, calibrate accelerometer/gyro sensors, bind the ELRS receiver, test motor direction, and conduct bench testing before attaching propellers for flight trials.

The Onshape file containing the 3D-printable drone frame can be found here:
https://cad.onshape.com/documents/d5cbef43a62eba2e76499c05/w/7bd8871aca8072e02db1bab7/e/778a021562ded3d7515ce905?renderMode=0&uiState=6a80d3db860458379a651e88

Within this project so far, I have referenced information I have learnt from a variety of Youtube videos, online forums and websites. I have also used GrabCad, an online database of open source CAD files to guide me through how to sketch, extrude and assembly the frame. Within the onshape file is the final result, however the version I 3D-printed may not be useable due to its low melting point - which makes use of any low/medium grade solder redundant. For this reason, I believe opting for a similar pre-made carbon fibre frame may be more prone to success.
