Out tool shelf consist of set of tools which can be used at the current visible objects in 3D viewport.

[[images/SCS_Tools_Shelf.png]]


### Tool Shelf

**Add Root**

Creates a new SCS Root Object. If there is any selection, it will automatically set these objects for SCS Game Object content by parenting it to the SCS Root Object.


**Add Root (with name request)**

Creates a new SCS Root Object. User can specify a name for the Root object in a window, that will appear. If there is any selection, it will automatically set these objects for SCS Game Object content by parenting it to the SCS Root Object.


### Convex

**Make Convex**

Makes a new object from selected Model objects. This new object is always convex and can be used as a base for convex colliders.


**Convert to Locator**

Converts selected objects into a new Collider Locator. There are additional choices for deleting of source object(s) – Delete Original Geometry, and for creating a single Locator or multiple Locators from every selected object – Individual Objects.


**Convert to Mesh**

Converts selected Collision Locator(s) into editable Model (Mesh) object(s).


### Visibility Tools

Visibility tools consists of sub-panel for viewing objects by type and three additional visibility operators.

**Switching by type**

[[images/SCS_Tools_Shelf_Op_Table.png]]

First table alters visibility of Model and Locators objects. Second table is used only for Prefab Locators.


**Global vs. SCS Root**

This option switches scope of visibility operators in this sub-panel. When using _**Global**_ operators will be applied among all of the objects in current scene, in the case of _**SCS Root**_ only the objects within current SCS Game Object will be altered.

**Current SCS Root**

Additional operators for switching visibility of objects within the SCS Game Object of active object:
* _**Invert Visibility**_ - inverts visibility of all objects.
* _**View All**_ - shows all objects.
* _**Isolate**_ - show all objects within SCS Game Object of active object and hide all other objects in scene.


### Display Methods


**Glass Objects**

* _**Wires / Textured**_ - two operators for quick setting of the drawing type for all Glass objects in the scene.


_**Shadow Casters**_

* _**Wires / Textured**_ - two operators for quick setting of the drawing type for all Shadow caster objects in the scene.


**Collision Locators**

* _**All Wires / No Wires**_ - operators to quickly turn ON or OFF all the wires in all Collision Locators in the scene.

* _**All Faces / No Faces**_ - operators to quickly turn ON or OFF all the faces in all Collision Locators in the scene.


### Lamp Switcher and Lamp UV Tool

Tools shelf also include lamp tools which are described in [[Lamp Tools]] section.