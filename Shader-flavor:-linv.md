Flavor inverting liminance mixing used on luminance shaders of [[shader type: dif.lum.spec]].

Luminance shaders without this flavor usually lit surfaces where base texture alpha channel is 255 and don't lit on surfaces with alpha value 0, however shaders using this flavor invertes that behaviour (alpha value 0 gives full lit and alpha value 255 no lit).