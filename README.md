# VQEngine - A DirectX11 & C++11 Real-Time Renderer

![](Data/Icons/VQEngine-icon.png) 

A DirectX 11 rendering framework for stuyding and practicing various rendering techniques and real-time algorithms. 



###### BRDF, Environment Lighting, Directional Lights, PCF Shadows

![](Screenshots/objs3.PNG)

###### Model Loading (.obj), Sponza Scene, SSAO, HDR, Bloom

![](Screenshots/models2.PNG)

###### Debug Rendering, CPU & GPU profiler, Frame Stats, Bounding Boxes

![](Screenshots/debug.PNG)

###### SSAO w/ Gaussian Blur

![](Screenshots/SSAO.gif)

# Feature List / Version History

See [Milestones](https://github.com/vilbeyli/VQEngine/milestones) for the planned upcoming changes and [Releases page](https://github.com/vilbeyli/VQEngine/releases) for the version histroy.

## What's Next

The latest changes can be found in the [dev branch](https://github.com/vilbeyli/VQEngine/tree/dev), or another branch named with the feature being implemented. _These branches might be unstable before the release_.

**[v0.5.0](https://github.com/vilbeyli/VQEngine/releases/tag/v0.5.0) - Performance Optimization & Debugging Enchancements** - TBA
 
 - Performance Optimizations
 - ASSAO & Render Quality Settings
 - Instanced Rendering
 - Frustum Culling
 - Cached Environment Maps
 - Improved Stability

## Released

 **[v0.4.0](https://github.com/vilbeyli/VQEngine/releases/tag/v0.4.0) - Data-Oriented Engine, Multi-threaded Tasking System, Model Loading w/ assimp, Loading Screen** - July15-2018
 - Refactored Scene, Engine and Renderer classes in favor of [Data-Oriented Design](https://en.wikipedia.org/wiki/Data-oriented_design)
 - Asynchronous Model Loading using [assimp](https://github.com/assimp/assimp)
 - [Sponza](http://www.crytek.com/cryengine/cryengine3/downloads) Scene & More Models
 - Task-based Threading System
 - Rendering: Directional Lights, Alpha Mask Textures
 - Loading Screen & Multi-threaded Scene Loading
 - App Icon
 - Documentation, Resource Collection & Wiki Pages

 **[v0.3.0](https://github.com/vilbeyli/VQEngine/releases/tag/v0.3.0) - Automated Build, Logging, Text Rendering, CPU & GPU Profiler** - May7-2018
 - Text Rendering
 - CPU & GPU Profiler
 - Shader Binary Cache
 - Build scripts (Python, Batch) & Automated Build (AppVeyor)
 - Logging: Console and/or Log Files

 **[v0.2.0](https://github.com/vilbeyli/VQEngine/releases/tag/v0.2.0) - PBR, Deferred Rendering & Multiple Scenes** - December1-2017
 - On-the-fly-switchable Forward/Deferred Rendering
 - PBR: GGX-Smith BRDF
 - Environment Mapping (Image-Based Lighting)
 - PCF Soft Shadows
 - Bloom
 - SSAO w/ Gaussian Blur
 - Custom Scene Files, Switchable/Reloadable Scenes

**[v0.1.0](https://github.com/vilbeyli/VQEngine/releases/tag/v0.1.0) - Phong Lighting, Shadow Mapping, Texturing and Shader Reflection** - July15-2017
 - Vertex-Geometry-Pixel Shader Pipeline
 - Shader Reflection
 - Phong Lighting
 - Point/Spot Lights
 - Simple Shadow Mapping Algorithm for Spot Lights
 - Normal/Diffuse Maps
 - Procedural Geometry: Cube, Sphere, Cylinder, Grid
  
# Prerequisites

The projects are set to build with the following configurations:

 - [Windows 10 SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk) - 10.0.16299.0
 - Visual Studio 2017 - v141, v140
  
- **GPU**: Radeon R9 380 equivalent or higher. Demo hasn't been tested on other systems. Feel free to [open an issue](https://github.com/vilbeyli/VQEngine/issues) in case of crashes / errors.

# Build

![https://ci.appveyor.com/api/projects/status/8u0a89j15naw0jlp/branch/master?svg=true](https://ci.appveyor.com/api/projects/status/8u0a89j15naw0jlp/branch/master?svg=true)

Run `BUILD.bat` or `BUILD.py` to build the project. `./Build/_artifacts` will contain the VQEngine executable built in release mode and the data and shaders needed to run the demo. You need Visual Studio 2017 installed for the build scripts to work.


# Controls

| Scene Controls |  |
| :---: | :--- |
| **WASD** |	Camera Movement |
| **R** | Reset Camera |
| **C** | Cycle Through Scene Cameras |
| **Shift+R** |	Reload Current Scene From File |
| **0-5** |	**Switch Scenes**: <br>**1**: Objects Scene <br>**2**: SSAO Test <br>**3**: Environment Map Test <br>**4**: Stress Test <br>**5**: Sponza Scene

| Engine Controls |  |
| :---: | :--- |
| **Page Up/Down** | Change Environment Map |
| **;** |	Toggle Displaying CPU/GPU Performance Numbers |
| **'** / **Shift + '** |	Toggle Displaying Rendering Stats / Renderer Controls |
| **Backspace** | Pause App |
| **ESC** |	Exit App |

| Renderer Controls | |
| :---: | :--- |
| **F1** |	Toggle Forward/Deferred Rendering |
| **F2** |	Toggle Ambient Occlusion |
| **F3** |	Toggle Bloom |
| **F4** |	Toggle Display Render Targets |
| **F5** |  Toggle Bounding Box Rendering |

# 3rd Party Open Source Libraries
 
 - [nothings/stb](https://github.com/nothings/stb)
 - [freetype-windows-binaries](https://github.com/ubawurinna/freetype-windows-binaries)
 - [DirectXTex](https://github.com/Microsoft/DirectXTex)
 - [assimp](https://github.com/assimp/assimp)