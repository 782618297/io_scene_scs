Lamp system uses "lamp" material effect to visualize extra lit surfaces by second mask texture or by alpha channel of base texture. This system is used on vehicle lights, vehicle auxiliary lights and traffic lights.

## Vehicle lights

Vehicle lights uses second mask texture where each channel from RGBA color space defines mask for particular type of the light:
* R - left blinker, right blinker
* G - high beam, brake
* B - low beam, reverse, daytime running (DRL)
* A - positional

Second requirement for vehicle lights to work is separate UV layer for lamp mask texture and proper tile offset of the mappings. Tilling is applied on the right side of the texture in the following order:

1. original texture - front left side of vehicle
2. first texture tile - front right side of vehicle
3. second texture tile - rear left side of vehicle
4. third texture tile - rear right side of vehicle
5. fourth texture tile - middle of vehicle and DRL


## Lamp tools

Blender Tools implements "Lamp Switcher" and "Lamp UV Tool" for previewing and properly mapping meshes which uses lamp material.


### Lamp switcher

Lamp switcher is preview tool for switching ON and OFF different type of lights in all currently created materials. Lamp switcher can be found in 3D view under SCS Tools panel and consist of three groups:
* **Vehicle** - used for switching vehicle lights
* **Auxiliary**  - used for switching vehicle auxiliary lights
* **Traffic Lights** - used for switching traffic lights

> NOTE: To see changes in 3D view you should use GLSL shading mode and use at least one lamp material on at least one object.
  
[[images/SCS_Tools_Shelf_-_Lamp_Switcher.png]]


### Lamp UV Tool

Lamp UV Tool is helper tool for positioning UV mappings of selected faces on active UV layer. You can use the tool only in "Edit Mode" of mesh objects. Tool will automaticly reposition selected faces to proper texture tile depending on what lamp type was selected. Similary as Lamp Switcher UV tool has three groups:
* **Vehicle** - UV mappings are positioned depending on vehicle side.
* **Auxiliary** - UV mappings are positioned depending on the lit color of auxiliary.
* **Traffic Lights** - similarly as in auxiliary UV mappings are positioned depending on the type of traffic light.

[[images/SCS_Tools_Shelf_-_Lamp_UV_Tool.png]]

When hitting any of the buttons tool will take currently selected faces and set offset for UV mappings on active UV layer according to property and type of light.