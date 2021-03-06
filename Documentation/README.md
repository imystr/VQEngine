# VQEngine Documentation

This page is Currently to serve as a collection of resources that influenced the engine/renderer design.

# Engine Design

Below is the collection of resources used for building the VQEngine.

## Conference Talks & YouTube Content

- [CppCon2017: Nicolas Guillemot “Design Patterns for Low-Level Real-Time Rendering”](https://www.youtube.com/watch?v=mdPeXJ0eiGc)
- [GCAP 2016: Parallel Game Engine Design - Brooke Hodgman](https://www.youtube.com/watch?v=JpmK0zu4Mts)
- [CppCon 2016: Jason Jurecka “Game engine using STD C++ 11"](https://www.youtube.com/watch?v=8AjRD6mU96s)
- [C++Now 2018: Allan Deutsch "Game Engine API Design"](https://www.youtube.com/watch?v=W3ViIBnTTKA)
- [CppCon 2014: Mike Acton "Data-Oriented Design and C++"](https://www.youtube.com/watch?v=rX0ItVEVjHc)
- [Jonathan Blow: Data-Oriented Demo: SOA, composition](https://www.youtube.com/watch?v=ZHqFrNyLlpA)
- [Code Blacksmith: Thread Pool Tutorial](https://www.youtube.com/watch?v=eWTGtp3HXiw)

## Text

- [Game Programming Patterns](http://gameprogrammingpatterns.com/contents.html)
  - [Data Locality](http://gameprogrammingpatterns.com/data-locality.html)
  - [Object Pool](http://gameprogrammingpatterns.com/object-pool.html)

# Rendering

## BRDF

- [Joe DeVayo: LearnOpenGL - PBR Theory](https://learnopengl.com/#!PBR/Theory)
- [PBS Physics Math Notes](http://blog.selfshadow.com/publications/s2012-shading-course/hoffman/s2012_pbs_physics_math_notes.pdf)
- [Trowbridge-Reitz GGX Distribution - How NDF is defined](http://reedbeta.com/blog/hows-the-ndf-really-defined/)
- [Fresnel-Schliick w/ roughness](https://seblagarde.wordpress.com/2011/08/17/hello-world/)

## Depth Buffer
  - [NVidia - Depth Precision Visualized](https://developer.nvidia.com/content/depth-precision-visualized)
  - [The Devil In The Details: Linear Depth](http://dev.theomader.com/linear-depth/)
  - [Robert Dunlop: Linearized Depth using Vertex Shaders](https://www.mvps.org/directx/articles/linear_z/linearz.htm)
  - [Emil "Humus" Persson: A couple of notes about Z](http://www.humus.name/index.php?ID=255)
  - [MJP: Reconstructing Position From Depth](https://mynameismjp.wordpress.com/2009/03/10/reconstructing-position-from-depth/)
  - [David Lenaerts: Reconstruction Positions From the Depth Buffer](http://www.derschmale.com/2014/01/26/reconstructing-positions-from-the-depth-buffer/)

## Rendering Math
- [gamedev StackExchange QA: Cylindrical Projection UV Coordinates](https://gamedev.stackexchange.com/questions/114412/how-to-get-uv-coordinates-for-sphere-cylindrical-projection)
- [Paul Bourke: Converting to/from Cube Maps](http://paulbourke.net/miscellaneous/cubemaps/)

- Hammersley Sequence - Quasi-Monte Carlo
   - [Holger Dammertz - Hammersley Points on the Hemisphere](http://holger.dammertz.org/stuff/notes_HammersleyOnHemisphere.html )
   - [Scratchapixel: Introduction to Quasi Monte Carlo](https://www.scratchapixel.com/lessons/mathematics-physics-for-computer-graphics/monte-carlo-methods-in-practice/monte-carlo-methods)


## VQEngine Architecture


VQEngine architecture is more or less based on [Nicolas Guillemot's CppCon2017 Talk:  “Design Patterns for Low-Level Real-Time Rendering”](https://www.youtube.com/watch?v=mdPeXJ0eiGc).

![](renderer-design.PNG)

## Misc Figures

![](commands.PNG)
![](mem-man-discrete.PNG)
![](mem-man-integrated.PNG)

