Locators are used for placing of special items to the “SCS Game Model”.
To create a Locator the first thing you have to do is to create an Empty object (**Shift+A → Empty → \<any type>**).

[[images/SCS_Tools_Locators_01.png]]

Now while the object is active go to the Object Properties tab in Properties window and find “SCS Object Specials” palette. Here is the “SCS Objects” sub-palette, where you can change the Object Type. Change it to Locator type.

[[images/SCS_Tools_Locators_02.png]]

Now you can choose from three types of Locators in the Locator Type drop-down menu: Prefab, Model and Collision.

> NOTE: Prefab and Collision locators are not fully supported yet!


### Model Locators

Model Locators can be used to place an existing game models to other game model without the need to include their data physically in host file. Simply said, these models are only referenced in the host file. This way you can for example define a places in a truck model, where mirrors or other upgrades will appear in the game by player's will.

[[images/SCS_Tools_Locators_-_Model_02.png]]


**Name**

This property here is the same as Blender Object's name and will be used by game engine (e. g. in the model of wheels for ETS2, "bb" is the name of the locator which represents size of the wheel).

**Hookup**

This property can be set according to records in “Hookup Library” (see the chapter “Path Settings” in [[Global Settings]]).

> NOTE: Model Locators can also use "Preview Model" feature (see the chapter “Preview Models”).


### Collision Locators

Collision locators are used for simulation of realistic physical interactions between objects in game. There are four types of primitives: "Box", "Sphere", "Capsule" and "Cylinder". Beside primitives there is also special type of collision locator named "Convex" which uses convex geometry instead.

Each locator object has it's own display options which will set rendering mode of locator in 3D view. You can switch rendering of wire frame ("Wireframes") and shell ("Faces") of locator.

First property that will reflect exported data is "Locator Centered", which will position locator primitive to center when used.

All types also features physical property "Mass Weight" which specifies mass of the object.


**Box**

[[images/SCS_Tools_Locators_Collision_1Box_01.png]]

* "X/Y/Z Dimension" - size of the body on each axis.


**Sphere**

[[images/SCS_Tools_Locators_Collision_2Sphere_01.png]]

* "Sphere Diameter" - size of the sphere.


**Capsule**

[[images/SCS_Tools_Locators_Collision_3Capsule_01.png]]

* "Capsule Diameter" - size of the capsule ending.
* "Capsule Length" - length of the capsule body.


**Cylinder**

[[images/SCS_Tools_Locators_Collision_4Cylinder_01.png]]

* "Cylinder Diameter" - diameter of cylinder.
* "Cylinder Length" - length of cylinder body.


**Convex**

[[images/SCS_Tools_Locators_Collision_5Convex_01.png]]

* "Collision Margin" - scales the convex envelope by the same distance on all axis.

Convex locator features additional info line which tells you how many vertices is in this convex locator.

For easy convex locator creation, please see the section [[SCS Tools in Shelf#convex]].

> NOTE: Keep in mind that convex locator should have really small amount of vertices (ideally up to 64 vertices) because of expensive calculations in game.


### Preview Models on locators

When you use Locators which represents some other models, it is often handy to see those models directly on Locator's position, so you can see how the whole unit will looks like. It can be done with use of Preview Models functionality. It is available for Model and Prefab Locators.

[[images/SCS_Tools_Locators_Preview_Model_01.png]]


**Preview Model**

Here you can navigate to the PIM file. Its geometries are then loaded to the locator's position to preview target model's shape.


**Show Preview Model**

Here you can turn displaying of already loaded Preview Model ON or OFF.


**Draw Type**

Drop-down menu enables to change the drawing type for the Preview Model. The choices are “Wire”, “Solid” and “Bounds”. Please note, that “Textured” drawing mode has not much of sense here, since the materials for Preview Models are not loaded at a time.

> NOTE: You can also disable/enable displaying of all Preview Models in the scene using the global option “Show Preview Models” in the Display Settings sub-palette.
> 
> [[images/SCS_Tools_Locators_Preview_Model_03.png]]