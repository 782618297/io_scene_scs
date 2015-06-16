Animations used in SCS games are driven by skeletons and keyframes animations deforming bones in the skeleton. There are two types of these animations:

1.  **Program driven animations** which mostly expects animation range from 0 to 1 if not stated differently in animation definition files. This means that first frame will be used as 0 state and last frame will be used as state 1 any state between this range is interpolated across whole keyframes range of animation. Example of this animations are truck interior animations in Euro Truck Simulator 2 which are defined inside each truck definition folder (example path: "def/vehicle/truck/man.tgx/interior/animations.sui").

2. **Static loop animations** used by so called "mover" objects. Movers can be placed all around the game world with the help of map editor. Examples for mover objects are: windmills, pedestrians, animals etc. To create your own mover you should create new "def/world/mover.<id_of_your_mod>.sii" file and define mover in there by the template from original "def/world/mover.sii" file.
> NOTE: Special type of movers named "walkers" can also use forward movement in their animation which can be animated as movement of skeleton object on Y axis.

Regardless on the usage of the SCS Animation, creation pipeline within Blender Tools is the same for both above types. To create SCS Animation you will have to use standard Blender procedure of armature creation and pose rigging and then set it up in SCS Animations panel. It is also important to know, that only: location, rotation and scale manipulation of bones will be exported during SCS Animation export.


# SCS Animations Panel

To export created skeleton pose animation into the game you will also have to use SCS Animations panel which you can find in object properties. The panel will appear only if the currently selected object is armature.

[[animations panel picture]]

> NOTE: When seeing "No 'SCS Root Object'!" message instead of animations list make sure to parent armature object to SCS Root Object.


### Custom Export Path

First property of animations panel that you can set is custom export path which you shall use if you would like to store your animation files somewhere else than rest of the exported files. This path may be useful when you are creating sequence of animations for walkers, as all of your walkers can use the same skeleton and animations and thus you may export them in different directory.

If custom path remains disabled all of the SCS Animations will be exported beside the rest of the exported files.


### SCS Animations List

Next you will find SCS Animations list where all animations used on current SCS Game Object are listed. For creation or deletion of SCS Animations use [[+]] and [[-]] buttons on the side of the animations list. Furthermore animations can be imported with [[importbutton]]  button, which will place you into file browser to select SCS Animation for importing.

Each SCS Animation entry features: 
* name of SCS Animation which will be also used as the name of exported animation file (PIA), 
* export operator [[exportbutton]] for exporting only animation used in that line,
* export inclusion property, which will decline export of animation used in that line when it's unticked and you are exporting whole SCS Game Object.


### Active Animation Settings

This panel area is actual place where you link Blender action (animation) to currently selected SCS Animation in list and set various properties for it.

Properties of SCS Animation:
* **Start** - frame in action which will be used as a start of SCS Animation,
* **End** - frame in action which will be used as an end of SCS Animation,
* **Length** - animation duration in seconds,
* **Increase Animation Step [[increasebutton]]** - stretches action by factor 2 and increases ***Export Step*** by one to compensate scaling. This gives you better control on sub keyframes and distribution of transformations over time,
* **Decrease Animation Step [[decreasebutton]]** - shrinks action by factor 2 and decreases ***Export Step*** by one to compensate scaling. This removes each second keyframe which decreases control over the whole animation,
* **Export Step** - number of frames to step in Blender action for each iteration on export.


### Animation Player


# SCS Skeleton Panel



