Same as [[shader type: dif.spec]] with one more texture which color and alpha is multiplied with base texture. 

Example usage in Euro Truck Simulator 2 is trailer where company texture is multiplied with base texture of the trailer.


### Useful Flavor Combinations

1. **"dif.spec.mult.dif.spec.tsnmap.shadow"** - beside normal maps geometries with this material will also cast shadows. This type of shader shall be used only in the case of complex animated geometries, because cost of animation calculation may be greater than calculating shadows directly on high poly mesh.
