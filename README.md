# Vulkan_Ray_tracing
-----

# Real-Time Ray Tracing Renderer (Vulkan)

## 📖 Overview

This project is a real-time ray tracing renderer built from scratch using C++ and the **Vulkan API**. The goal is to generate photorealistic images by leveraging modern rendering techniques and the high performance of Vulkan.

This project showcases the ability to design complex 3D rendering pipelines, implement GPU-accelerated ray tracing, and perform performance optimizations.

-----

## ✨ Key Features

  * **Real-Time Ray Tracing**: Implemented using Vulkan's `VK_KHR_ray_tracing_pipeline` extension to render realistic lighting effects like shadows and reflections in real-time.
  * **Real-Time Denoising**: Applied a **compute shader-based Denoising filter** to significantly improve image quality by removing noise from the ray-traced results in real-time.
  * **3D Model Loading**: Capable of loading various 3D model formats such as `.obj` and `.gltf`, including their materials, using the `Assimp` library.
  * **User Interface (GUI)**: Implemented a GUI with `Dear ImGui` to control rendering options, camera settings, and model information in real-time.

-----

## 🛠️ Tech Stack & Libraries

  * **Language**: C/C++
  * **Graphics API**: **Vulkan**
  * **Key Libraries**:
      * `GLFW`: Window creation and input handling
      * `GLM`: Mathematical operations
      * `Dear ImGui`: User interface
      * `Assimp`: 3D model loading
      * `stb_image`: Image file loading

-----

## ⚙️ Build & How to Run

### Requirements

  * A GPU that supports ray tracing (NVIDIA RTX 20 series or newer, AMD RX 6000 series or newer)
  * Latest graphics drivers
  * Vulkan SDK
  * Windows / Visual Studio 2019 or later

### Build Steps

1.  Clone the repository.
    ```bash
    git clone https://github.com/your-username/vulkan_ray_tracing.git
    cd vulkan_ray_tracing
    ```
2.  Open the `rtrtFramework/src/rtrt.sln` file in Visual Studio.
3.  Set the solution configuration to `Release` or `Debug` and the platform to `x64`.
4.  Build the project by selecting `Build > Build Solution`.
5.  Once the build is complete, run `rtrt.exe` from the `rtrtFramework/src/x64/Release/` folder.

-----

## 👨‍💻 Project Structure

```
vulkan_ray_tracing/
├── rtrtFramework/
│   ├── libs/         # External libraries (GLFW, GLM, ImGui, etc.)
│   ├── src/
│   │   ├── shaders/  # GLSL shaders (Ray Generation, Hit, Miss, Denoise, etc.)
│   │   ├── spv/      # Compiled SPIR-V shaders
│   │   ├── models/   # 3D models used for rendering
│   │   ├── app.cpp   # Main application logic
│   │   └── vkapp* # Core Vulkan initialization and rendering pipeline code
│   └── ...
└── README.md
```

-----

## 💡 Future Work

  * [ ] Improve PBR shaders for various materials (e.g., glass, metal)
  * [ ] Implement Global Illumination
  * [ ] Support for animated models

-----

## 📞 Contact

  * **Name**: Wonhyeong Chae
  * **Email**: wchae7@gmail.com
