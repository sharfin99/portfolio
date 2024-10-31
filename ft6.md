## Low-Cost 6-Axis Force/Torque Sensor for Robot Hands

[<a href="https://arxiv.org/abs/2410.03481">Paper</a>][<a href="https://youtu.be/QZGhIQBNQCY">Video</a>]

Force/torque sensing is an important modality for robotic manipulation, but commodity solutions, generally developed with other applications in mind, do not generally fit the needs of robot hands. We use LEDs mounted on two plates connected by a transparent elastomer to sense displacement between the plates and relate it to applied forces and torques. This method allows for a compact, fully integrated package at a low manufacturing cost.

<video src="images/FT_Optic_ICRA (online-video-cutter.com).mp4" width="480" height="240" controls></video>


### 1. Concept

<img src="images/2D_Deformation_of_a_6axis_sensor-1.png?raw=true"/>

We align two PCBs with LEDs directly above each other. We attach these circuit boards to rigid plates, we then suspend both of these plates in a translucent, elastic material. Assuming the bottom plate is fixed, a force applied to the top plate will displace the plate and change how to emitter LED shines on the receiving LED. The displacement will change the receiving signal, which we then will use in a data-driven approach to relate back to the force applied.

### 2. Design

<img src="images/complete_design_fig_2-1.png?raw=true"/>

Our F/T sensor is composed of two custom PCBs that have both LED emitters and clusters of LED receivers. When the top and bottom PCB boards are aligned directly above each other, our sensor has 3 total emitter-receiver pars. The PCBs are fastened to rigid, 3-D printed plates. The plates are then fixed above each other in a mold that we then fill with PDMS. Once cured, the two PCBs are suspended above each other in a solid cylinder of 10:1 PDMS. We use a single FFC connector to communicate between the top and bottom board. We use an additional FFC connector on the bottom board to communicate with external electronics. The rigid plates are fitted with threaded holes to mount external hardware.



