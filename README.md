# TouchDesigner Workshop USC 2026

![gif](readme-assets/media-04.gif)

## Dependencies

* Workshop TouchDesigner version - 2025.32460
  * [downloads page](https://derivative.ca/download)
* TouchDesigner MediaPipe plugin
  * [releases page](https://github.com/torinmb/mediapipe-touchdesigner/releases)
    

# Workshop Overview

This short 2-hour workshop will give an introduction to TouchDesigner via a crash-course in network building, working with different operator families, and exploring realtime inputs via the [TouchDesigner Mediapipe plugin](https://github.com/torinmb/mediapipe-touchdesigner).

This repo contains all of the exercises we've gone over together in the workshop, along with additional examples to learn more of the fundamentals of TouchDesigner. 

To see a step-by-step walkthrough of the first couple of excercises check out the following blog posts:

* [Is this TouchDesigner?](https://www.zoesandoval.com/blog/2026/3/24/is-this-touchdesigner)
* [Is this Interactivity?](https://www.zoesandoval.com/blog/2026/3/24/is-this-interactivity)
  
<br>

  
![image](readme-assets/media-01.png)

<br>

## Navigating the Evironment

The first time you open any new application it can be frustrating or confusing as you try to understand how the interface works. TouchDesigner is a node based toolkit, and while it's similar to many tools, it's also distinctly unique. We'll take a little time to cover the basics of getting around the environment, and how to understand what we're seeing. Before you know it you'll be zooming around your networks like it's second nature.

> Half of learning a new tool or development environment is just figuring out where all the knobs and buttons are. In this first course we’ll focus on getting your bearings in TouchDesigner, learning the essential interface elements and controls, as well as the fundamental principles of each operator family.

Learn more at [Navigating the TouchDesigner Environment](https://learn.derivative.ca/courses/100-fundamentals/lessons/101-navigating-the-environment/)

<br>

## Operator Families

![image](readme-assets/op-families-01.png)

Operators are the building blocks of our TouchDesigner networks. In a typically TouchDesigner project you'll find a series of operators connected by wires into a network. These networks make up the code for your project. The operators in our networks are separated into families which also represent that kinds of data that they contain.

### [Working with TOPs](https://learn.derivative.ca/courses/100-fundamentals/lessons/102-tops-working-with-images/)

### [Working with CHOPs](https://learn.derivative.ca/courses/100-fundamentals/lessons/103-chops-working-with-signals/)

### [Working with SOPs](https://learn.derivative.ca/courses/100-fundamentals/lessons/104-sops-rendering-3d-scenes/)

### [Working with DATs](https://learn.derivative.ca/courses/100-fundamentals/lessons/107-dats-scripting-python/)

### [Working with COMPs](https://learn.derivative.ca/courses/100-fundamentals/lessons/105-comps-interfaces-organization-outputs/)


<br>

## Interactivity & Using Channel Data

![image](readme-assets/media-02.gif)

### Connecting Families

While it’s great to see how we connect operators of like families together, most of the work we do with TouchDesigner often requires connecting operators of different families together. We’ll look at simple examples of how we can start building relationships between operators of different families, and how we can use these ideas to build responsive and interactive networks.

### TouchDesigner MediaPipe Plugin

We'll also take a look at how we can work with [TouchDesigner Mediapipe plugin](https://github.com/torinmb/mediapipe-touchdesigner) in our projects: from downloading it from the main repo, optimizing for project performance, smoothing and manipulating sensor data, to simple techniques for realtime hand-tracking.

![image](readme-assets/media-03.png)

<br>

## Realtime Rendering

We'll pull all of our elements together to render them in a simple scene that overlays a butterfly on our webcam, and shows how we can transform the butterfly into a swirl of noisey magic. 

![image](readme-assets/media-04.gif)

<br>

> Real time rendering in TouchDesigner requires a few primary ingredients. These are made up of both Component Operators, Texture Operators, and Surface Operators. Our most basic set-up starts with a [Light](https://docs.derivative.ca/Light_COMP), [Camera](https://docs.derivative.ca/Camera_COMP), and [Geometry COMP](https://docs.derivative.ca/Geometry_COMP). Component operators can hold entire networks, and the Geometry COMP typically holds the SOPs we plan on rendering. In order to actually render our scene we need to add a [Render TOP](https://docs.derivative.ca/Render_TOP) to our network. The Render TOP uses the Light, Camera, and Geo COMPs to create a 2D view of our 3D scene.

Learn more at [TouchDesigner Basic Render Setup](https://learn.derivative.ca/courses/100-fundamentals/lessons/104-sops-rendering-3d-scenes/topic/basic-render-setup/)

<br>

----

# Resources

* [Learn TouchDesigner from Derivative]
* [The Interactive & Immersive HQ]
* [TouchOSC]
* [OSC]
* [Visual Studio Code]
* [Derivative Blog]
* [TouchDesigner MediaPipe Plugin]

<!-- links -->

[Learn TouchDesigner from Derivative]: https://learn.derivative.ca/
[The Interactive & Immersive HQ]:https://interactiveimmersive.io/
[System Requirements]: https://docs.derivative.ca/index.php?title=System_Requirements
[TouchDesigner 099]: https://derivative.ca/download
[Derivative Registration]: https://derivative.ca/user/register
[Visual Studio Code]: https://code.visualstudio.com/
[Derivative Blog]: https://derivative.ca/showcase
[TouchDesigner MediaPipe Plugin]: https://github.com/torinmb/mediapipe-touchdesigner
