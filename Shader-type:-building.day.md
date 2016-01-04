Same as [[shader type: building.add.env.day]] without reflection component.

It effectively switches two materials depending on the time of the day. During the day it uses [[shader type: dif.spec]] material where alpha is used as specular map and at night switches to [[shader type: dif.lum.spec]] in order for windows to light at the night.