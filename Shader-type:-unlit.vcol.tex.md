Similar to [[shader type: unlit.tex]] with additional multiplication by vertex color.

As for transparent flavor combinations this shader uses vertex color alpha multiplied with base texture alpha channel.

### Useful Flavor Combinations

* **"unlit.vcol.tex.a.over"** - is useful for animated indicators of dashboard inside truck in Euro Truck Simulator 2, as alpha over flavor combination makes transparent areas where texture alpha channel or vertex color is 0.