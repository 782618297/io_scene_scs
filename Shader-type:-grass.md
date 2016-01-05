Shader used in special cases for static not moving grass.

It's result is the same as [[shader type: dif]] with transparency controlled by multiplication between vertex alpha color and base texture alpha channel.

Normals on the meshes using this shader are ignored as shader always uses normals up as lighting applied to mesh should more-or-less match the ground.