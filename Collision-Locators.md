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