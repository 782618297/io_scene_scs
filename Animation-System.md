Animations used in SCS games are driven by skeletons and keyframes animations deforming bones in the skeleton. There are two types of these animations:

1.  **Program driven animations** which mostly expects animation range from 0 to 1 if not stated differently in animation definition files. This means that first frame will be used as 0 state and last frame will be used as state 1 any state between this range is interpolated across whole keyframes range of animation. Example of this animations are truck interior animations in Euro Truck Simulator 2 which are defined inside each truck definition folder (example path: "def/vehicle/truck/man.tgx/interior/animations.sui").

2. **Static loop animations** used by so called "mover" objects. Movers can be placed all around the game world with the help of map editor. Examples for mover objects are: windmills, pedestrians, animals etc. To create your own mover you should create new "def/world/mover.<id_of_your_mod>.sii" file and define mover in there by the template from original "def/world/mover.sii" file.
> NOTE: Special type of movers named "walkers" can also use forward movement in their animation which can be animated as movement of skeleton object on Y axis.

Regardless on the usage of the SCS Animation, creation pipeline within Blender Tools is the same for both above types. To create SCS Animation you will have to use standard Blender procedure of armature creation and pose rigging and then set it up in SCS Animations panel. It is also important to know, that only: location, rotation and scale manipulation of bones will be exported during SCS Animation export.


# SCS Animations Panel

To export created skeleton pose animation into the game you will also have to use SCS Animations panel which you can find in object properties. The panel will appear only if the currently selected object is armature.

[[animations panel picture]]

> NOTE: When seeing "No 'SCS Root Object'!" message instead of animations list make sure to parent armature object to SCS Root Object.

For creation or deletion of SCS Animations [[+]] and [[-]] buttons on the side of the animations list can be used. 

### Custom Export Path

As usually 

# SCS Skeleton Panel



