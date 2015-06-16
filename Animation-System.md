Animations used in SCS games are driven by skeletons and keyframes animations deforming bones in the skeleton. There are two types of these animations:

1.  **Program driven animations*** which mostly expects animation range from 0 to 1 if not stated differently in animation definition files. This means that first frame will be used as 0 state and last frame will be used as state 1 any state between this range is interpolated across whole keyframes range of animation. Example of this animations are truck interior animations in Euro Truck Simulator 2 which are defined inside each truck definition folder (example path: "def/vehicle/truck/man.tgx/interior/animations.sui").

2. **Static loop animations** used by so called "mover" objects. Movers can be placed all around the game world with the help of map editor. Beside animating skeleton bones, mover animation can also contain movement curve of the whole skeleton which is in game used as path curve. Examples for mover objects are: windmills, pedestrians, animals etc. To create your own mover you should create new "def/world/mover.<id_of_your_mod>.sii" file and define mover in there by the template from original "def/world/mover.sii" file.


Both types of animation are anyway treated the same within Blender Tools so procedure for animation creation and export is the same.

