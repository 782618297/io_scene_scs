SCS Blender Tools uses its own Material settings, so every Material in Blender contains a palette called “SCS Materials”. It is essential to use settings here exclusively to set up any available Material properties. If you'll be changing the Material's settings in Blender's standard palettes, the appearance of the Material will change in 3D View, but the SCS material settings will not change and exported material may look very different when viewed in SCS Game Engine.

`NOTE: Unfortunately, it is not possible to see in current “SCS Blender Tools” implementation the same looking shaders in Blender as it will appear later in SCS Game Engine. This is because Blender uses different shader models then SCS Game Engine and the implementation is just trying to get the visuals as close as possible using current Blender shaders.`

The settings for SCS Material can be created from one of two types:

* **Imported Shader**

  [[images/SCS_Material_Imported_Shader.png]]

  When you import any existing game model and some of the material effects cannot be found in existing Shader Presets, Imported Shader is created. Attributes cannot be edited, but it will still export correctly as it was in original file. Though textures and their mappings can be changed.

* **Shader Preset**

  [[images/SCS_Material_Shader_Preset.png]]

  The “SCS Materials” palette features the list of Shader Presets, where you can choose from materials with its own predefined values and change some of them to your liking. Shader Presets can be found as a collapsible list, which is loaded from the Shader Presets Library file (see the chapter “Path Settings” in [[Global Settings]]).


**Substance**

Item from list of physical materials, which is loaded from Material Substance Library file (see the chapter “Path Settings” in [[Global Settings]]). These can for example set up the physical type of the road surface.


**Material Attributes**

In this section you can find various visual shader attributes, that you can alter. Most important ones are interactively reflected on your model in 3D View.


**Material Textures**

This section provides an interface for specifying texture images for different shader's texture channels. Most prominent textures are automatically loaded and displayed in the 3D View.

Each texture features:
* **Texture**
  
  Setting this property will open file browser where you will be able to select image for this texture. After selecting, the image will be automatically applied to material.

* **Mapping**

  This property specifies which UV layer will be used for this texture. For some textures you may need to specify more then one UV layer, depends on which Shader Preset is used.
  
  `NOTE: if more UV layers are needed only first one is used in Blender 3D viewport but all of them are used on export.`

* **Export TOBJ**

  TOBJ files are pointers to texture images and are by default exported if they don't exist yet. If you manually tick _**Export TOBJ**_, then texture object file will be always exported with selected settings.

  _**Settings**_ are in fact set of boolean options:
    * _**U Repeat**_ - repeat texture in U direction.
    * _**V Repeat**_ - repeat texture in V direction.
    * _**TS Normal**_  - tangent space normal for the texture.
    * _**No MIP Maps**_ - don't use MIP Maps for the texture.
    * _**No Compress**_ - don't use compression on texture.
