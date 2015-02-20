As Blender Tools are still in development below is the list of currently supported shaders.

1. "building.add.env.day" - used for windows on buildings. 
2. "dif.a" - most basic shader with diffuse light featuring one texture. The areas on geometries where texture has alpha value 0 will be transparent.
3. "dif.spec" - basic shader with diffuse and specular light featuring one texture. Alpha of the texture represents intensity of specular light.
4. "dif.spec.a" - same as "dif.spec" with extra feature of making transparent areas where texture has alpha with value 0.
5. "dif.spec.add.env" - same as "dif.spec" with extra texture for reflection used for vehicles.
6. "dif.spec.add.env.nofresnel" - same as "dif.spec.add.env"
7. "dif.spec.weight" - 
8. "fakeshadow" - 
9. "shadowonly" - used on geometry for shadow casting.