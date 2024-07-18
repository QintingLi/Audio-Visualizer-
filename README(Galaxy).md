#Introduction

Sonic Pulsar is an innovative audio visualizer powered by three.js, GLSL, and JavaScript. This cutting-edge application seamlessly combines audio processing with 3D graphics rendering capabilities, bringing sound to life with mesmerizing visuals that pulsate and dance in tune with the rhythm. 

Users can select their audio source and immerse themselves in various visualizer options:

* Galaxy: A dynamically generated 3D galaxy composed of particles that synchronize their movements with musical data, resulting in a realistic visualization of the Milky Way.

* 2D: Experience a lively graphical dance of shapes and colors responding to every note in the audio.

* Sphere: Marvel at a spherical visual spectacle that twists and undulates, reacting to the ebb and flow of your selected music.

* Cubes: Watch a sea of cubes ripple and resonate with the beat, creating a stunning rhythmic mosaic.

* Orbs: Dive into a mesmerizing soundscape of orbs that bubble, burst, and form to the rhythm.

* Raymarching: Explore geometric landscapes evolving with the music, delivering a unique psychedelic experience.

* Jelly: Discover a whimsical, jelly-like world that wriggles and writhes in tune with the audio.

  Sonic Pulsar isn't limited to live events. Accepting inputs from various audio sources, including Spotify and Soundcloud, it can be your personal visual companion for private jam sessions, study times, or moments of relaxation. 

Looking ahead, Sonic Pulsar holds endless possibilities, including integrating machine learning algorithms to adapt visuals to your musical taste, connecting with AR/VR platforms for an immersive multi-sensory experience, or evolving into an artistic tool for digital creators. Sonic Pulsar goes beyond being an app; it's a new way to experience music. Plug in your favorite track, lean back, and let Sonic Pulsar transform your audio experience into a visual delight.



##Galaxy - Project Overview

The Galaxy Visualization Project is a 3D simulation of a galaxy created using [Three.js](https://threejs.org/). The project features a visually appealing representation of a galaxy with various stars and particles. Users can interact with the galaxy and visualize it from different perspectives. The simulation uses WebGL for rendering and employs custom shaders and textures to enhance the visual experience.



Technology Stack

- Three.js

Purpose: Serves as the core 3D graphics library.
Functionality: Enables the creation and rendering of geometries, materials, textures, and light sources.

- JavaScript

Purpose: Provides the scripting language for implementing interactive logic, animations, and event handling.
Functionality: Controls the dynamic behavior of the celestial bodies and handles user interactions.

- HTML/CSS

Purpose: Constructs the structure and style of the web interface.
Functionality: Ensures a responsive and visually appealing layout for the simulation environment.

- WebGL

Purpose: Provides the rendering context for hardware-accelerated 3D graphics.
Functionality: Delivers high-performance rendering capabilities necessary for real-time simulations.

- Detector Object

Purpose: Detects the availability of WebGL in the user's browser.
Functionality: Provides user feedback and guidance if WebGL is not supported, ensuring a smooth user experience.



Key Features

**Astro Class**:

- **Definition**: Encapsulates the properties and behaviors of celestial bodies.

- **Attributes**: Includes radius, texture URL, distance from a reference point, rotation velocities, and lighting conditions.

- Methods

  :

  - `model()`: Creates the 3D model of the celestial body using sphere geometry and appropriate materials.
  - `animate()`: Updates the rotation and orbital motion based on defined velocities.
  - `addSatellite()`: Adds a satellite (e.g., moon) to the celestial body, managing hierarchical relationships.



**Lighting Simulation**:

- **Basic and Phong Materials**: Differentiates between illuminated and non-illuminated celestial bodies.

- **Light Sources**: Adds point lights to simulate stars or other light-emitting bodies, enhancing realism.

  

**Animation and Interactivity**:

- **Rotational and Orbital Dynamics**: Simulates realistic celestial mechanics.

- **User Controls**: Enables interactive control over the simulation, such as pausing rotations via mouse clicks.

  

**Error Handling and Guidance**:

- **WebGL Detection**: Checks for WebGL support and provides user guidance for enabling it if necessary.



Implementation Details

- Geometry and Materials:

- Sphere Geometry: Defines the shape of celestial bodies.
  Texture Mapping: Applies realistic textures to celestial bodies using image files.
  Shadow Casting: Controls whether a celestial body casts shadows, depending on its lighting condition.
  Object Hierarchies:

- Object3D Containers: Manages hierarchical transformations, such as rotations and translations, for complex motion patterns.
- Transform Groups: Organizes the different layers of transformations for each celestial body.
  Performance Optimization:

- Efficient Rendering: Utilizes WebGL's hardware acceleration for smooth and responsive visuals.
  Adaptive Animations: Ensures that animations remain fluid even on less powerful devices.

  