Lamp system uses "lamp" material effect to visualize extra lit surfaces by second mask texture or by alpha channel of base texture. This system is used on vehicle lights, vehicle auxiliary lights and traffic lights.

## Vehicle lights

Vehicle lights uses second mask texture where each channel from RGBA color space defines mask for particular type of the light:

* R - left blinker, right blinker
* G - high beam, brake
* B - low beam, reverse, daytime running (DRL)
* A - positional

Second requirement for vehicle lights to work properly is separate UV layer for lamp mask texture and proper tile offset of the mappings. Tilling is applied on the right side of the texture in the following order:

1. original texture - front left side of vehicle
2. first texture tile - front right side of vehicle
3. second texture tile - rear left side of vehicle
4. third texture tile - rear right side of vehicle
5. fourth texture tile - middle of vehicle and DRL


## Auxiliary lights

Auxiliary lights on vehicles can also have separate second mask texture but they use only two channels from light mask texture:

* R - dimmed beam
* G - full beam
* B - not used and must be zero (black)
* A - not used and must be zero (black)

There is also possible to use two different colors for auxiliary lights with offsetting UV mappings for second mask texture. Tile offset here is also done on the right side of the texture:

1. original texture - white color
2. first texture tile - orange color


## Traffic lights

Traffic lights don't use extra second mask texture as they are using alpha channel of base texture for proper lit of traffic lights. But they still use tile offset on UV mappings to properly lit up different color in traffic light. Tile offset here is done on right up side of the texture in the following order:

1. first texture tile - red color of traffic light
2. second texture tile - yellow color of traffic light
3. third texture tile - green color of traffic light


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

Lamp UV Tool is helper tool for positioning UV mappings of selected faces on active UV layer. This tool will help you easily position uv mappings on the proper tile of texture depending on vehicle side or auxiliary lamp color or traffic light color. You can use this tool only in "Edit Mode" of mesh objects. Tool will automatically reposition selected faces to proper texture tile depending on what lamp type was selected. Similarly as Lamp Switcher UV tool has three groups:
* **Vehicle** - UV mappings are positioned depending on vehicle side.
* **Auxiliary** - UV mappings are positioned depending on the lit color of auxiliary.
* **Traffic Lights** - similarly as in auxiliary UV mappings are positioned depending on the color of traffic light.

[[images/SCS_Tools_Shelf_-_Lamp_UV_Tool.png]]

When hitting any of the buttons tool will take currently selected faces and set offset for UV mappings on active UV layer according to property and type of light.