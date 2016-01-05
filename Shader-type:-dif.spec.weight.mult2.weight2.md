Same shader family as [[shader type: dif.spec.weight.mult2]] with additional layer of second base and multiplication texture.

Fading between first and second layer of base & multiplication texture is done by vertex color alpha, where value 0 will use only first layer and value 0.5 will use only second layer, any value in-between will mix both layers respectively.

Usually this extended shader is used for simulating transitional areas on the edge of the road.