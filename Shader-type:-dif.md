This is one of the most basic shader with diffuse and specular light featuring one texture. Specular light is used directly from value specified in material.

### Extensions
1. **"dif.a"** - the areas on geometries where texture has alpha value 0 will be transparent. Example usage: grills, railings and ladders on far buildings.
2. **"dif.shadow"** - uses geometry also as shadow caster. This type of shader shall be used only in the case of complex animated geometries, because cost of animation calculation may be greater than calculating shadows directly on high poly mesh.
3. **"dif.shadow.a"** - is a combination of "dif.shadow" and "dif.a" which means that areas of geometry which will be transparent also won't cast shadows. This shader may be used for fences models which shall beside begin transparent also cast shadows.
4. **"dif.over"** - in this case alpha map represent transparency blending of material, where alpha with value 0 means completely transparent and alpha with value 255 means non transparent.