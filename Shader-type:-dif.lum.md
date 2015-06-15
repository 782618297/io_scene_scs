Same as [[shader type: dif]] with additional linear interpolation calculation between "dif" shader result and base texture RGB colors by factor of base texture alpha channel. As a result this shader will give you lit surfaces during the night, where amount of surface lit is donated by base texture alpha channel.

Example usage of this shader are dashboard and gps surfaces in truck inside Euro Truck Simulator 2 game.

### Extensions

1. **"dif.lum.decal.over"** -  decal part of shader name donates ability to use lightning model from the surfaces lying behind geometries using this shader and over part of shader name represent transparency blending of material, where alpha with value 0 means completely transparent and alpha with value 255 means non transparent. Example usage of this shader are lit icons on buttons in truck cabin which shall be: 
   1. lit to reflect effect of back light,
   2. transparent around icon to blend on the button below,
   3. use the lightning model from the surface below again for blending on the button surface.