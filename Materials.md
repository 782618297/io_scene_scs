SCS Blender Tools uses its own Material settings, so every Material in Blender contains a palette called “SCS Materials”. It is essential to use settings here exclusively to set up any available Material properties. If you'll be changing the Material's settings in Blender's standard palettes, the appearance of the Material will change in 3D View, but the SCS material settings will not change and exported material may look very different when viewed in SCS Game Engine.

### Lamps and 3D View setup

To get closest result to the one in SCS Game Engine you should use one "Sun" lamp with settings shown in the image below. 

[[images/SCS_Material_Specials_-_Lamp_Setup.png]]

Additionally you have to switch shading in the 3D view properties to GLSL and tick "Backface Culling" to see models properly.

[[images/SCS_Material_Specials_-_3D_View_Setup.png]]


### Shader Types

The settings for SCS Material can be created from one of two types:

* **Shader Preset**

  [[images/SCS_Material_Specials_-_Shader_Preset.png]]

  The “SCS Materials” palette features the list of Shader Presets, where you can choose from materials with its own predefined values and change some of them to your liking. Shader Presets can be found as a collapsible list, which is loaded from the Shader Presets Library file (see the chapter “Path Settings” in [[Global Settings]]).

* **Imported Shader**

  [[images/SCS_Material_Specials_-_Imported_Shader.png]]

  When you import any existing game model and some of the materials cannot be found in existing Shader Presets, Imported Shader is created. Attributes cannot be edited, but it will still export correctly as it was in original file. Though textures and their mappings can be changed for visual preview.
  
  Additionally there is "Mappings" field inside "Textures" for this type of shader. "tex_coord_X" entries specify which UV layer will be exported for this alias.


### Properties and usage

Properties in material are shader type dependent. So each type of shader may have different attributes and textures. Additionally there is "WT" button for some of the properties which can be written through all of the looks, for more information see the section [[Look System#write-through]]

**Substance**

Substance property is item from list of physical materials, which is loaded from Material Substance Library file (see the chapter “Path Settings” in [[Global Settings]]). These can for example set up the physical type of the road surface.


**Material Attributes**

In this section you can find various visual shader attributes, that you can alter. Most important ones are interactively reflected on your model in 3D View.


**Material Textures**

This section provides an interface for specifying texture images for different shader's texture channels. Most prominent textures are automatically loaded and displayed in the 3D View.

Each texture features:
* **Texture**
  
  Setting this property will open file browser where you will be able to select image (only *.tga image file format is officially supported) for this texture. After selecting, the image will be automatically applied to material.

  > NOTE: using image out of SCS project directory (see [[Global Settings#path-settings]]) and it's subdirectories may cause errors and warnings on export!

  Each texture also features extra row of controls for TOBJ file and it's settings. TOBJ files are pointers to texture images and are by default created upon export if they don't exist yet. However create button ( [[images/SCS_Material_Specials_-_Create_TOBJ_Btn.png]] ) will appear if TOBJ file doesn't exist yet and pressing it will create TOBJ file for this texture with default settings. In case this texture already has TOBJ file there will be only reload button ( [[images/SCS_Material_Specials_-_Reload_TOBJ_Btn.png]] ) with which you can load currently saved settings of this TOBJ. Sometimes reload button may appear in red color which indicates that current settings are outdated and you should press reload button to reload them. As soon as TOBJ file exist you will also have access to change any value in settings itself. Changing any of the setting in settings list will rewrite TOBJ file with updated values right away.

 _**Settings**_ of TOBJ file are:
    * _**U Repeat**_ - repeat texture in U direction.
    * _**V Repeat**_ - repeat texture in V direction.
    * _**TS Normal**_  - tangent space normal for the texture.
    * _**No MIP Maps**_ - don't use MIP Maps for the texture.
    * _**No Compress**_ - don't use compression on texture.


* **Mapping**

  This property specifies which UV layer will be used for this texture. For some textures you may need to specify more then one UV layer, depends on which Shader Preset is used.
  
  > NOTE: if more UV layers are needed only first one is used in Blender 3D viewport but all of them are used on export.`