# Voxel Cube Renderer

This project is a simple voxel cube renderer using OpenGL, GLFW, and GLEW. The program displays a grid of colored cubes in a 3D space, allowing for interaction through mouse movement and scroll to zoom.

## Features

- **Rendering**: Renders a grid of `50x50x50` cubes, each with a unique color generated based on its index.
- **Camera Controls**: Allows for camera movement through mouse interaction.
  - **Mouse Movement**: Rotates the camera around the scene.
  - **Scroll**: Zooms the camera in and out.
- **Lighting**: Implements basic Phong lighting with ambient, diffuse, and specular components.

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

# TODO List for Voxel Cube Renderer

This document outlines future improvements and features that can be added to enhance the functionality and performance of the Voxel Cube Renderer.

## Features

- [ ] **Instancing**:Implement instancing to improve performance when rendering a large number of cubes.
- [ ] **Implement Dynamic Voxel Addition/Removal**: Allow users to add or remove voxels interactively, enabling more flexible scene modifications.
- [ ] **Voxel Selection**: Implement functionality to select and highlight individual voxels with the mouse.
- [ ] **Save/Load Scenes**: Add support for saving and loading voxel configurations to/from files.
- [ ] **Advanced Lighting**: Introduce more sophisticated lighting techniques such as shadow mapping or bloom effects.
- [ ] **Textures and Materials**: Allow voxels to be textured with images or procedural patterns to enhance visual fidelity.
- [ ] **Multiple Light Sources**: Add support for multiple dynamic light sources with adjustable properties.


## Performance Improvements

- [ ] **Frustum Culling**: Implement frustum culling to avoid rendering voxels outside the camera's view.
- [ ] **Level of Detail (LOD)**: Use LOD techniques to optimize rendering performance for distant voxels.
- [ ] **Multithreading**: Explore multithreading options to improve rendering and input responsiveness.

## Usability Enhancements

- [ ] **GUI Integration**: Incorporate a graphical user interface using libraries like ImGui for easier interaction and control.
- [ ] **Customization Options**: Provide user options for customizing voxel colors, lighting settings, and grid size.
- [ ] **Camera Controls**: Enhance camera controls with features like reset view, snapping, and preset camera angles.

## Code Quality

- [ ] **Refactor Code**: Organize the codebase for better readability and maintainability.
- [ ] **Error Handling**: Improve error handling and logging for easier debugging.
- [ ] **Unit Tests**: Add unit tests to verify the correctness of key functionalities.

## Documentation

- [ ] **In-depth Documentation**: Expand the existing documentation to include a comprehensive user guide and developer reference.
- [ ] **Tutorials and Examples**: Provide tutorials and example scenes to help new users get started.

## Research

- [ ] **Explore Voxel Compression Techniques**: Investigate methods for compressing voxel data to reduce memory usage.
- [ ] **Investigate Alternative Shading Models**: Research and experiment with other shading models that might offer better performance or visual quality.

---

This list is intended to guide the development of the Voxel Cube Renderer. Contributions are welcome, and suggestions for additional features or improvements can be added to this list.

