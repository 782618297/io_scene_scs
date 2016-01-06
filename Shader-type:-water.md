Shader composed of two independently scrolling water wave layers with added environmental reflection and near/horizon water color interpolation. First water wave is defined with layer0 texture, second with layer1 texture.

However shader also features a lot of extra parameters:

1. Distances:
  * Near - distance of interpolation start
  * Far - distance of horizon
  * Scramble - water surface distorts the reflection and scramble factor tells the amount of distortion
2. Near Color - base water color
3. Horizon Color - water color on horizon
4. Layer0 - first wave settings:
  * Yaw - wave layer orientation defined by counter-clockwise degree rotation around vertical axis
  * Speed - wave layer flow speed in meters per second
  * ScaleX - wave layer texture generation U scale factor
  * ScaleY - wave layer texture generation V scale factor
5. Layer1 - second wave settings:
  * Yaw - wave layer orientation defined by counter-clockwise degree rotation around vertical axis
  * Speed - wave layer flow speed in meters per second
  * ScaleX - wave layer texture generation U scale factor
  * ScaleY - wave layer texture generation V scale factor