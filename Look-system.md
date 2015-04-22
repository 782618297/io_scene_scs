Looks in SCS games are used to define same model with different textures or material attributes. With this system you can easily extend your model to have several looks without exporting same geometry over and over again. Examples of typical look usage in SCS games are: gas stations, trailers, depot companies etc.

So each SCS Game Object inside Blender file has it's own definitions for looks. You can create, delete and edit look names in "SCS Looks" box under "SCS Objects Specials" panel when SCS Root Object is active or "SCS Material Specials" panel when mesh object is active.

[[images/SCS_Tools_Object_Specials_-_SCS_Looks.png]]

To change material attributes or textures for some look, you have to select it in the list shown above and then just change the material attributes. Now whenever you will change active look all of the materials in current SCS Game Object will be updated with values from this look and you will also be able to see the changes in 3D view.

> NOTE: Using same material in multiple SCS Game Objects will adopt materials to values in currently selected SCS Game Object. With that in mind any meshes with this material in other SCS Game Objects won't be displayed properly, but still they will be properly exported.


### Write Trough

Most of SCS material settings can be "written trough" which means that the current value of setting is written to all looks. This way you can for example easily change texture which you want to use in all looks without selecting each look and searching for the texture over and over again.

Write trough button is founded before material setting value marked as "WT" as in the image below.

[[images/SCS_Material_Specials_-_WT.png]]