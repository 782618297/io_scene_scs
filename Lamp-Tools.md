Blender Tools implements "Lamp Switcher" and "Lamp UV Tool" for previewing and properly mapping meshes which uses lamp material.


## Lamp switcher

Lamp switcher is preview tool for switching ON and OFF different type of lights in all currently created materials. 

When switching ON any type of the light you will see brighten surfaces on the meshes using lamp material. If you don't see any change in 3D view there is either problem in UV mapping of the meshes or the mask texture is not properly created. Lamp switcher can be found in 3D view under SCS Tools panel and consist of three groups:
* **Vehicle** - used for switching vehicle lights
* **Auxiliary**  - used for switching vehicle auxiliary lights
* **Traffic Lights** - used for switching traffic lights

> NOTE: To see changes in 3D view you should use GLSL shading mode and use at least one lamp material on at least one object.
  
[[images/SCS_Tools_Shelf_-_Lamp_Switcher.png]]


## Lamp UV Tool

Lamp UV Tool is helper tool for positioning UV mappings of selected faces. Tool will reposition mappings on the UV layer used by mask texture in lamp material. 

You can use this tool only in "Edit Mode" of mesh objects. By pressing any of the buttons tool will automatically reposition selected faces UV mappings to proper texture tile depending on selected vehicle side or auxiliary lamp color or traffic light color. Similarly as Lamp Switcher, UV tool also has three groups:
* **Vehicle** - UV mappings are positioned depending on vehicle side.
* **Auxiliary** - UV mappings are positioned depending on the lit color of auxiliary.
* **Traffic Lights** - similarly as in auxiliary UV mappings are positioned depending on the color of traffic light.

[[images/SCS_Tools_Shelf_-_Lamp_UV_Tool.png]]