# ModernOpenglCube

# Voxel Cube Renderer

This project is a 3D visualization tool that renders a grid of voxel cubes using modern OpenGL. It includes functionality for real-time interaction, such as zooming and rotating the view.

## Features

- **Voxel Grid Rendering**: Renders a grid of 50x50x50 colored cubes using instancing for performance optimization.
- **Interactive Controls**: Supports mouse and scroll interactions for rotating the scene and zooming in/out.
- **Lighting and Shading**: Implements basic ambient, diffuse, and specular lighting models for realistic shading.
- **Random Colors**: Generates random colors for each cube to create a visually engaging experience.

## Requirements

- **C++ Compiler**: Ensure you have a modern C++ compiler that supports C++11 or later.
- **OpenGL Libraries**: Requires the following libraries:
  - [GLFW](https://www.glfw.org/): Used for window creation and input handling.
  - [GLEW](http://glew.sourceforge.net/): Used for managing OpenGL extensions.
  - [GLM](https://github.com/g-truc/glm): Used for matrix and vector operations.

## Setup and Installation

1. **Install Dependencies**:
   - Make sure to have GLFW, GLEW, and GLM installed on your system.
   - On Ubuntu, you can install them using:
     ```bash
     sudo apt-get install libglfw3-dev libglew-dev
     ```
   - On Windows, you can download the binaries from their respective websites and add them to your project.

2. **Build the Project**:
   - Use the following command to compile the project:
     ```bash
     g++ -s -o voxel_renderer -O2 main8.cpp -lglfw -lGLEW -lGL -lGLU
     ```

3. **Run the Executable**:
   - Execute the compiled binary:
     ```bash
     ./voxel_renderer
     ```

## Usage

- **Mouse Control**: 
  - Move the mouse to rotate the view.
  - Scroll to zoom in and out.
- **Window Resize**: The viewport adjusts automatically when the window is resized.

## Code Overview

- **main8.cpp**: Contains the main logic for setting up the OpenGL context, rendering loop, and input handling.
- **Shaders**: 
  - Vertex and fragment shaders are embedded as C++ string literals for ease of distribution.

## Troubleshooting

- Ensure your graphics drivers are up-to-date.
- Make sure all dependencies are properly installed and linked.
- If you encounter errors related to GLEW initialization, ensure you have a compatible OpenGL context.

## License

This project is open source and available under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.
