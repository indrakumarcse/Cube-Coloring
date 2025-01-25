Interactive 3D Icosahedron Grid 🌌
This project is an interactive 3D grid of Icosahedrons, built using Three.js. It allows users to interact with the grid by hovering over individual objects, dynamically changing their colors to random values. The project also features a gradient background and real-time performance monitoring.

Features ✨
Interactive Grid:
A 3D grid of Icosahedrons created using THREE.InstancedMesh for optimized rendering.
Dynamic color changes upon hovering over the objects.

Gradient Background:
A custom gradient background from purple to dark blue, enhancing the visual aesthetics.

Dynamic Parameters:
Easily control the grid size through the URL query parameter (e.g., ?15 for a 15×15×15 grid).
Includes a GUI for adjusting instance count interactively.

Optimized Performance:
Efficient rendering with instanced geometry.
Real-time performance stats via Stats.js.

Smooth Controls:
Orbit controls with damping for a user-friendly camera experience.

Demo 🌐
You can host this project using platforms like Vercel or GitHub Pages.

How It Works 🔍

Grid Initialization:
A grid of Icosahedrons is created using THREE.InstancedMesh to optimize performance for thousands of objects.
The size of the grid can be modified via URL parameters (default is 10×10×10).

Dynamic Interactions:
Raycaster is used to detect mouse hover over the 3D objects.
Objects change to a random color upon hover, ensuring a unique interaction every time.

Background and Lighting:
The scene background is a gradient texture created dynamically using the canvas API.
A hemisphere light is added for soft, natural illumination.

Real-Time Updates:
The animate loop ensures the scene is updated continuously for smooth interactions.

Installation and Setup 🛠️
Prerequisites

A modern browser with WebGL support.
A local or online server for serving files (optional for advanced features).

Steps to Run
Clone the repository:

git clone https://github.com/your-username/3D-Icosahedron-Grid.git

Navigate to the project directory:

cd 3D-Icosahedron-Grid
Open the index.html file in a browser, or use a local server for an enhanced experience.

Adjust Grid Size
To change the grid size, append a number to the URL query string:

Example: index.html?15 will create a 15×15×15 grid.
Code Overview 📋
Key Libraries:

Three.js: For 3D rendering.

OrbitControls: For intuitive camera interaction.

Stats.js: For real-time performance monitoring.

Lil-GUI: For an interactive user interface.

File Structure:
index.html: The main entry point of the application.

script.js: Contains the core logic for scene creation and interactivity.
Core Functionalities:

Gradient Background:
A custom gradient is created using the canvas API and applied as the scene's background texture.
Raycasting:
Detects and interacts with objects based on mouse movements.

Dynamic Updates:
Objects change colors dynamically when hovered over.

