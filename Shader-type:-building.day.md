Use this material if you want your building windows to reflect at day-time and be lit at night. It shall be more or less used on distant "panorama" buildings as they don't need advanced features from [[shader type: window.day]] / [[shader type: window.night]].

It effectively switches two materials depending on the time of the day. During the day it uses [[shader type: dif.spec]] material where alpha is used as specular map and at night switches to [[shader type: dif.lum.spec]] in order for windows to light at the night. 

The base texture must have alpha channel on places where it should emit light at night.