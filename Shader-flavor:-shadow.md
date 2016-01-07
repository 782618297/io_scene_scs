Flavor enabling shadow casting pass on shader.

As there is separate shadow caster [[shader type: shadowonly]], this flavor should be used exceptionally. Usually can be used on animated models where cost of animation calculation on extra shadow caster mesh may be greater then calculating shadow caster directly from "high" poly mesh.