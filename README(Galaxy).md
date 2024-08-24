# Sonic Pulsar: A Next-Gen Audio Visualizer

## Introduction

Welcome to **Sonic Pulsar**, an innovative audio visualizer that merges advanced audio processing with dynamic 3D graphics, powered by three.js, GLSL, and JavaScript. This cutting-edge application transforms sound into stunning visual experiences, making music come alive through captivating visuals that respond to every beat and rhythm.

With Sonic Pulsar, users can select their audio source and explore a range of mesmerizing visualizations:

- **Galaxy**: Dive into a dynamically generated 3D galaxy of particles that move in perfect sync with the music, creating a stunning representation of the Milky Way.
- **2D**: Enjoy a vibrant display of shapes and colors that dance in response to every note.
- **Sphere**: Watch as a spherical form morphs and pulses, reflecting the flow of your chosen track.
- **Cubes**: Experience a rhythmic mosaic of cubes that ripple and move with the beat.
- **Orbs**: Immerse yourself in a visual soundscape where orbs bubble, burst, and form along with the music.
- **Raymarching**: Journey through geometric landscapes that evolve with the music for a psychedelic experience.
- **Jelly**: Explore a whimsical world of jelly-like forms that wriggle and sway in harmony with the audio.

Sonic Pulsar is versatile, supporting various audio inputs, including popular platforms like Spotify and Soundcloud. Whether you're hosting a live event or enjoying a private jam session, Sonic Pulsar enhances every musical moment.

### Future Vision

The possibilities for Sonic Pulsar are endless. Future developments may include integrating machine learning algorithms to tailor visuals to your musical tastes, expanding into AR/VR platforms for a fully immersive experience, and becoming a creative tool for digital artists. Sonic Pulsar is more than an app; it's a revolutionary way to experience music. Simply select your favorite track, sit back, and let Sonic Pulsar turn your audio experience into a visual journey.

---

## Galaxy Visualization Project: Overview

The **Galaxy Visualization Project** is a 3D simulation that offers a visually engaging representation of a galaxy, created using Three.js. This project allows users to interact with a 3D galaxy model, view it from various perspectives, and experience a realistic simulation of star movements and celestial dynamics.

### Technology Stack

- **Three.js**: The core 3D graphics library used to create and render geometries, materials, textures, and light sources.
- **JavaScript**: The scripting language for implementing interactive logic, animations, and event handling.
- **HTML/CSS**: Provides the structure and styling for a responsive and visually appealing web interface.
- **WebGL**: Enables hardware-accelerated 3D graphics rendering for high-performance, real-time simulations.
- **Detector Object**: Checks the user's browser for WebGL support and provides guidance if not supported, ensuring a seamless user experience.

### Key Features

- **Astro Class**:
  - **Definition**: Manages the properties and behaviors of celestial bodies.
  - **Attributes**: Includes details like radius, texture URL, distance from a reference point, rotation velocities, and lighting conditions.
  - **Methods**:
    - `model()`: Creates a 3D model of the celestial body using sphere geometry and appropriate materials.
    - `animate()`: Updates rotation and orbital motion based on set velocities.
    - `addSatellite()`: Adds satellites, such as moons, maintaining hierarchical relationships.

- **Lighting Simulation**:
  - Utilizes both basic and Phong materials to differentiate illuminated from non-illuminated celestial bodies.
  - Incorporates point lights to simulate stars or other light-emitting bodies, adding depth and realism.

- **Animation and Interactivity**:
  - **Rotational and Orbital Dynamics**: Provides realistic simulations of celestial mechanics.
  - **User Controls**: Allows users to interactively control the simulation, such as pausing rotations with mouse clicks.

- **Error Handling and User Guidance**:
  - **WebGL Detection**: Ensures users are informed about their browser's capabilities and how to enable WebGL if needed.

### Implementation Details

- **Geometry and Materials**:
  - Uses sphere geometry for defining celestial bodies.
  - Applies realistic textures using image files.
  - Controls shadow casting to enhance visual realism.

- **Object Hierarchies**:
  - Utilizes `Object3D` containers for managing complex motion patterns through hierarchical transformations.
  - Organizes multiple transformation layers for each celestial body using transform groups.

- **Performance Optimization**:
  - Leverages WebGL's hardware acceleration for smooth, responsive visuals.
  - Implements adaptive animations to maintain fluidity even on devices with lower performance capabilities.
  - 
