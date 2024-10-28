## Scalable Minnimally Acutated Quasi-Passive Walker 

<img src="images/9812053-fig-1-source-large.gif?raw=true"/>

**Project description:** <br/>
Small bipedal robots have potential of navigating small spaces with a simpler body, and also could be used in film, toys, and other entertainment industries. Shrinking a bipedal walker means there is limited room for actuation, control, and sensing for both stability and motion control. Our goal is to leverage passive dynamics to create a minimally actuated and controlled bipedal walking model that can be shrunk to a centimeter-scale.

### 1. Concept

<video src="images/videoplayback-ezgif.com-video-cutter.mp4" width="640" height="360" controls></video>

Quasi-passive walkers leverage curved, spherical feet and actuators to create walkers with minimally complex designs and control schemes. The curved feed are crucial to the stability and forward motion. The feet are curved in the frontal plane so the robot can wobble back and forth. Once the robot generates a strong wobble, the feet gain clearance and are free to swing forward. In Tad McGeer's initial model for passive walking, the robot was put on a inclined slope to generate a forward leg swing and the wobble was initiated by a human. 

With our robot design, we use a single actuator per leg to both generate this wobble and encourage the legs to swing forward.

### 2. Design
<img src="images/ModelsNew3.png?raw=true"/>
Our walking model consists of 5 rigid bodies – a torso, two upper legs, and two spherical section feet. The hip joint is passive, but there is an actuated prismatic joint in each of the two leg.
<video src="images/walkervid-ezgif.com-resize-video.mp4" width="640" height="360" controls></video>
This actuation scheme results in the stance leg extended past nominal during the stance phase and retracted during the swing phase. During double stance, with a phase offset of 180◦, both legs are at the nominal length. The stance leg extending and the swing leg retracting allow for increased swing leg clearance.

### 3. Experimental Results


