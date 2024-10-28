## Scalable Minnimally Acutated Quasi-Passive Walker 

[<a href="https://ieeexplore.ieee.org/document/9812053">Paper</a>][<a href="https://www.youtube.com/watch?v=kECAdJEaJlk">Video</a>]


Small bipedal robots have potential of navigating small spaces with a simpler body, and also could be used in film, toys, and other entertainment industries. Shrinking a bipedal walker means there is limited room for actuation, control, and sensing for both stability and motion control.

<video src="images/walkervid-ezgif.com-resize-video.mp4" width="480" height="240" controls></video>
<br>
By leveraging the passive 3D dynamics, carefully designing the spherical feet, and changing the actuation scheme, we are able to produce a very simple 3D bipedal walking model that has a total of 5 rigid bodies and a single actuator per leg.
<br>

### 1. Concept

<video src="images/videoplayback-ezgif.com-video-cutter.mp4" width="480" height="240" controls></video>
Quasi-passive walkers leverage curved, spherical feet and actuators to create walkers with minimally complex designs and control schemes. The curved feed are crucial to the stability and forward motion. The feet are curved in the frontal plane so the robot can wobble back and forth. Once the robot generates a strong wobble, the feet gain clearance and are free to swing forward. In Tad McGeer's initial model for passive walking, the robot was put on a inclined slope to generate a forward leg swing and the wobble was initiated by a human. 

### 2. Design

<img src="images/ModelsNew3.png?raw=true"/>
<br>
With our robot design, we use a single actuator per leg to both generate this wobble and encourage the legs to swing forward. Our walking model consists of 5 rigid bodies – a torso, two upper legs, and two spherical section feet. The hip joint is passive, but there is an actuated prismatic joint in each of the two leg. 

<img src="images/FeetNew3.png?raw=true"/>
<br>
The geometry of the spherical feet is crucial to creating a stable walking gait. Our walker is unique in that the profiles of the two feet are not concentric. This design choice allows for a smooth transition between the feet as the robot rolls laterally. 


### 3. Experimental Results

<img src="images/ResultsCombo.png?raw=true"/>
<br>
We tested three different feet geometries with 2D sagittal and frontal plane models, derived using a lagrangian formulation. Our model with non-concentric spherical feet produced the most stable gaits at different leg extension amplitude and control frequencies. We validated our results on a real walker. For more detailed and visual look at our results, see the video linked at the top. 
