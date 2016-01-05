Transition shader between two shaders of [[shader type: dif]] where base texture presents texture for first shader and over texture presents texture for second shader.

Fading between the two is done by vertex color alpha, where value 0 will use only base texture layer and value 0.5 will use only over texture layer, any value in-between will mix both layers respectively.