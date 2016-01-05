Transition shader between two shaders of [[shader type: dif.spec.weight.mult2]] for simulating transitional areas (usually road shoulders).

Fading between first and second shader is done by vertex color alpha, where value 0 will use only first layer and value 0.5 will use only second layer, any value in-between will mix both layers respectively.

This shader shall be replaced with [[shader type: dif.spec.weight.weight.dif.spec.weight]] instead if possible.