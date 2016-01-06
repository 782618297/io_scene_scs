Truckpaint shader as the name suggests is the shader for truck color paint. Shader features combination of base and paintjob textures. The final result of this shader is dependent on configuration of the truck paint inside definition files as the shader supports different output types. If the truck is driven by the player, shader is configured by "paint job" definition file of the truck, otherwise truck paint is configured from AI truck colors palette.

Additionally "aux" parameters inside material are used only for preview purposes. Their usage in 3D view is dependent on truckpaint mode:

1. "Color mask" mode (when "colormask" flavor is used) where paintjob texture RGB channels are used to color mask base truckpaint output. Auxiliary attributes are used in 3D viewport as follows:
    * Paintjob R Color -> color masked with B channel of paintjob texture,
    * Paintjob G Color -> color masked with G channel of paintjob texture,
    * Paintjob B Color -> color masked with R channel of paintjob texture,
    * Paintjob Base Color -> base paintjob color.
2. "Airbrush" mode (when "airbrush" extension is used) uses paintjob texture as airbrush mask on base truckpaint output. Auxiliary attributes are used in 3D viewport as follows:
    * Paintjob Base Color -> base paintjob color.

> NOTE: There are two more modes "flipflake" and "airbrush.flipflake" which are not yet implemented inside 3D viewport but they can be defined inside definition files anyway, because no additional data have to be exported for them.


### Useful Flavor Combinations

1. **"truckpaint.altuv"** - exports alternative UV layer for paint job. Alternative UV layer has to be specified in paintjob texture.
    > NOTE: Not using this extension alternative UV  won't be exported and thus can not be used in definition files for paint job.

2. **"truckpaint.airbrush"** - uses paint job as airbrush mask. Paintjob texture is multiplied with base truck paint color by factor of paintjob texture alpha channel.
    > NOTE: May or may not be used, shader will give the same result as usage of this extension is specified in definition files and the extension doesn't effect exported data.

3. **"truckpaint.airbrush.altuv"** - combined "truckpaint.altuv" and "truckpaint.airbrush" extensions.

4. **"truckpaint.tsnmap"** - with extra texture defining normal maps. Both textures are using same UV layer.

5. **"truckpaint.tsnmap.altuv"** - with extra texture defining normal maps. Both textures are using same UV layer. Beside normal maps shader also features "truckpaint.altuv" extension.

6. **"truckpaint.tsnmap.airbrush"** - with extra texture defining normal maps. Both textures are using same UV layer. Beside normal maps shader also features "truckpaint.airbrush" extension.

7. **"truckpaint.tsnmap.airbrush.altuv"** - with extra texture defining normal maps. Both textures are using same UV layer. Beside normal maps shader also features "truckpaint.altuv" and "truckpaint.airbrush" extensions.

8. **"truckpaint.tsnmapuv"** -  with extra texture defining normal maps using it's own UV layer.

9. **"truckpaint.tsnmapuv.altuv"** -  with extra texture defining normal maps using it's own UV layer. Beside normal maps shader also features "truckpaint.altuv" extension.

10. **"truckpaint.tsnmapuv.airbrush"** -  with extra texture defining normal maps using it's own UV layer. Beside normal maps shader also features "truckpaint.airbrush" extension.

11. **"truckpaint.tsnmapuv.airbrush.altuv"** -  with extra texture defining normal maps using it's own UV layer. Beside normal maps shader also features "truckpaint.altuv" and "truckpaint.airbrush" extensions.