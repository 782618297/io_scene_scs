As Blender Tools are still in development below is the list of currently supported shaders.

1. **"building.add.env.day"** - used for windows on buildings with optimized reflection. Geometry will be lit at night by alpha channel value.
2. **"dif.a"** - one of the most basic shader with diffuse light featuring one texture. The areas on geometries where texture has alpha value 0 will be transparent. Example usage: grills, railings and ladders on far buildings.
3. **"dif.spec"** - basic shader with diffuse and specular light featuring one texture. Alpha of the texture represents intensity of specular light.
 The most used material without reflections.
4. **"dif.spec.a"** - same as "dif.spec" with extra feature of making transparent areas where texture has alpha with value 0.
5. **"dif.spec.add.env"** - same as "dif.spec" with extra texture featuring reflection used for vehicles.
6. **"dif.spec.add.env.nofresnel"** - same as "dif.spec.add.env"
7. **"dif.spec.weight"** - same as "dif.spec" with addition of multiplying vertex color value with specular light.
8. **"fakeshadow"** - clipping of projected volumetric shadow. Example are wheels where geometry with this material cuts out the area of volumetric shadow from the vehicle.
9. **"shadowonly"** - used on geometry for shadow casting.