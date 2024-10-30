## Hardware/Software Co-Optimization for Underactuated Kinematic Chains

[<a href="https://arxiv.org/abs/2405.14566">Paper</a>][<a href="https://www.youtube.com/watch?v=4R8eNC-VpFc">Video</a>]

**Project description:** <br/>
Determining an appropriate set of hardware parameters for underactuated transmissions is difficult - even for traditional taskbased co-optimization methods. In this paper, our goal is to implement a task-based design and policy co-optimization method for underactuated, tendon-driven trasnmissions.

### 1. Concept

Underactuated manipulators require a carefully designed transmission, often tendon-driven, to take advantage of a reduced number of actuators in the robot. Co-optimization, or the process of simultaneously searching the space of both hardware and control, is a possible solution to the problem of ensuring that a given hardware design is capable of a desired task. However, co-optimization of non-trivial tranmsissions is very difficult, especially for real hardware.

The fundamental difficulty of such approaches lies in formulating a co-design problem that a) enables the use of non-trivial controllers or policies, b) can be solved to an acceptable optimum point, c) guarantees that the final result can be physically realized in real hardware, and finally d) ensures that the optimized control policy also transfers to real hardware without substantial loss of performance





### 2. Co-Optimization of non-differentiable model parameters w/ Reinforcement Learning

<img src="images/eye-candy_co.png?raw=true"/>

We apply MORPH, an iterative training framework for design-control co-optimization using reinforcement learning. First we co-optimize both a control policy and a neural network proxy of the hardware model with a hardware loss and task loss, the hardware loss is computed from a more realistic physics based hardware model that can be differentiable or non-differentiable. Using the updated hardware neural network, we search for design parameters that match the physics-based model to the neural network proxy. 


### 3. Multi-Flexor transmission for efficient end-to-end task based optimization

<img src="images/iros_oral_pitch.png?raw=true"/>

We design a multi-flexor transmission that enables efficient end-to-end task based optimization. In extension, each link is passively driven by an elastic tendon that stretches over a pulley and is fixed to the previous link - this gives us two design parameters for each link - radius of the extension pulley and the preload elongation. The chain is driven in flexion by actuated, rigid tendons that are position controlled and route through all the links in the chain over idler pulleys - this gives us an additional hardware parameter which is the radius of the pulley. 



<img src="images/model_tendon1.png?raw=true"/>

If we use multiple tendons, we can span a multi-dimensional manifodl. However, designing the appropriate transmission to make this manifold smooth and sufficient for the task is difficult. We use Morph to co-optimize a three-link, two-actuator robot with our transmission design. 

