Basic shader with diffuse and specular light featuring one texture. Alpha of the texture represents intensity of specular light.


### Useful Flavor Combinations

1. **"dif.spec.a"** - making transparent areas where texture has alpha with value 0.
2. **"dif.spec.over"** - texture alpha channel also represent transparency blending of material, where alpha with value 0 means completely transparent and alpha with value 255 means non transparent.
3. **"dif.spec.shadow"** - uses geometry also as shadow caster. This type of shader shall be used only in the case of complex animated geometries, because cost of animation calculation may be greater than calculating shadows directly on high poly mesh.
4. **"dif.spec.shadow.a"** - with enabled shadow calculations over alpha channel which means that areas of geometry which will be transparent also won't cast shadows.
5. **"dif.spec.tsnmap.shadow"** - with extra texture defining normal maps and using geometries for shadow casters. Both textures are using same UV layer. This type of shader shall be used only in the case of complex animated geometries, because cost of animation calculation may be greater than calculating shadows directly on high poly mesh.