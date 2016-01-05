Shader mostly used for rocks where one texture can be used as base and detail one.

Shader is fading between base and detail texture with assumption that detail texture is representing details of base texture (sounds like fractals). Therefore base and detail textures should use same texture file which has to be self-similar.

However blending details are defined with auxiliary values where:
* From - detail texture fade out start, represented as z-distance in meters
* Range - detail texture fade range, represented in meters
* Bias - strength of detail texture mixing with base texture
* UV Scale - UV layer scale factor for detail layer (as shader shall be using same textures for base and detail, this factor comes handy as user can use only one UV layer for base & detail and then this factor represents how UV layer will be rescaled for detail texture)