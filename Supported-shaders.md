As Blender Tools are still in development below is the list of currently supported shaders.

1. **"building.add.env.day"** - use this material if you want your building windows to reflect at day-time and be lit at night. It effectively switches two materials depending on the time of the day. During the day is uses "eut2.dif.spec.add.env" material with texture for reflections and at night switches to "eut2.dif.lum.spec" in order for windows to light at the night. The texture must have alpha channel on places where it should have reflections and light at night.
2. **"dif.a"** - one of the most basic shader with diffuse light featuring one texture. The areas on geometries where texture has alpha value 0 will be transparent. Example usage: grills, railings and ladders on far buildings.
3. **"dif.spec"** - basic shader with diffuse and specular light featuring one texture. Alpha of the texture represents intensity of specular light.
 The most used material without reflections.
4. **"dif.spec.a"** - same as "dif.spec" with extra feature of making transparent areas where texture has alpha with value 0.
5. **"dif.spec.add.env"** - same as "dif.spec" with extra texture featuring reflection used for vehicles.
6. **"dif.spec.add.env.nofresnel"** - same as dif.spec.add.env, but it doesn't use fresnel computation, therefore is slightly cheaper to compute.
7. **"dif.spec.weight"** - same as "dif.spec" with modified specular light. It's mostly used for roads and asphalts, due distinct feel of specularity and diffuse properties of such surfaces.
8. **"fakeshadow"** - geometry with this material is used to outline contour of the vehicle from which casting of shadow volume begins. Due wheels vertical motion this material is required to be present in the wheel scene as well. It must outline the contour of the whole wheel.
9. **"shadowonly"** - used on geometry for casting sun shadows.