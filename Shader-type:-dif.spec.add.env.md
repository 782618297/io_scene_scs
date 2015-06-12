Same as [[shader type: dif.spec]] with extra texture featuring reflection used for vehicles.


### Extensions

1. **"dif.spec.add.env.paint"** - with usage of extra color defined in definition files. All white areas on the base texture will be masked with extra color while in game. This shader is either used for AI cars or truck parts which should be painted with base truck color.
2. **"dif.spec.add.env.tsnmap"** - with extra texture defining normal maps. Both textures are using same UV layer.
3. **"dif.spec.add.env.tsnmapuv"** - with extra texture defining normal maps using it's own UV layer.
4. **"dif.spec.add.env.nofresnel"** - without fresnel computation, therefore is slightly cheaper to compute.