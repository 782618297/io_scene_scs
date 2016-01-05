Transition shader between two shaders of [[shader type: dif.spec.weight]], where texture for first shader is presented as base and texture for second shader as over texture.

Fading between the two is done by vertex color alpha, where value 0 will use only base texture layer and value 0.5 will use only over texture layer, any value in-between will mix both layers respectively.

Additionally this shader also supports secondary specular (color and shininess), so even shaders with different specular behaviour can be transitioned.

This shader is usually primary choice when creating roads with transition to road shoulder.