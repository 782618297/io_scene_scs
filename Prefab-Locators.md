Prefab locators are used during the creation of prefab map assets. Examples of this assets are: roads, crosses, docking companies, services, gas stations etc. So purpose of prefab locators in this assets is to store data for AI traffic connection/rules, players interactions and GPS navigation. 

Because of different usage and data we have multiple types of Prefab Locators with their own set of properties described below.


## Control Node

Control Node is used: as prefab control in SCS map editor, as connection to other map assets and also as AI traffic entry/exit point. 

For proper prefab creation this requirements have to be meet:

1. Prefab must have from 2 to 6 control nodes;
2. Each control node has to have unique index, defined by "Node Index" property;
3. When creating more than 2 nodes, they have to be placed clockwise starting with index 0;
4. If prefab should be extended with in game generated terrain, then control node has to have terrain points assigned on it's left side.

[[/images/SCS_Tools_Locators_Prefab_CN.png]]

**Node Index** - property which defines index of the control node.

**Assign Terrain Points** - operator for assigning terrain points from mesh to the control node. For usage please use info icon on the left side of operator button.

**Clear All Terrain Points** - operator for clearing all terrain points from the control node.

**Preview Terrain Points [Visible|All]** - are operators for previewing currently assigned terrain points of the control node. ***Visible*** operator will show only assigned terrain points of currently visible mesh in 3D viewport; as for ***All*** will also preview any assigned terrain points from hidden mesh.


## Sign

Sign locator is exactly what names says: locator for placing signs on prefabs. With assigning "Sign Model" property from Sign Library it is decided which sign will appear on the place of locator in the game.

> NOTE: If you are not able to assign any sign to "Sign Model" property, make sure your Sign Library path is properly set.

[[/images/SCS_Tools_Locators_Prefab_SIGN.png]]

**Sign Model** - property defining sign id which shall be used in the game.


## Spawn Point

Spawn point locator defines point of different predefined players actions.

Example usage for company dock for Euro Truck Simulator 2 is creating at least two spawn points:

1. Spawn point of type "Company Point" which defines, check in point that player uses when he wants to select delivery;
2. 2nd spawn point of type "Unload (Easy)" which defines, the point to which user has to park trailer.

[[/images/SCS_Tools_Locators_Prefab_SP.png]]

**Spawn Type** - property defining type of spawn point.


## Traffic Semaphore

Traffic semaphore locators define stop and go actions for AI traffic. Primarily it's used for traffic lights but it can also be used for any other game defined profile, for example stopping AI car at gas station for fuel filling.

It's behaviour is defined by selected "Profile" and it's bind to user specified "ID". Selected "ID" is then used in "Navigation Points" to define effected AI traffic lane of this semaphore (check [Navigation Point](Prefab-Locators#navigation-point) for details).

Additionally user can specify "Type" property for defining of exceptional behaviour (use it only if you know what you are doing).

[[/images/SCS_Tools_Locators_Prefab_TS.png]]

**ID** - property defining ID of the semaphore.

**Profile** - property defining profile from Traffic Semaphore Library, which defines behaviour of traffic semaphore: intervals/distances and cycle delays.

> NOTE: If you are not able to assign any profile, make sure your Traffic Semaphore Library path is properly set.

**Type** - property defining semaphore type. In most cases "(use profile)" should be in use, meaning any intervals/distances and cycle delay will be defined by used profile from Traffic Semaphore Library.

**Intervals/Distances [G,O,R,O]** - intervals/distances for each state of traffic semaphore. Enabled only if you don't use "(use profile)" type of traffic semaphore.

**Cycle Delay** - property defining delay for which each semaphore cycle will be delayed before starting again. Enabled only if you don't use "(use profile)" type of traffic semaphore.


## Navigation Point

Navigation Point locators are used for creation of AI traffic lanes with curves. Because AI traffic lanes define driving paths for AI cars inside prefab, navigation point locators have to be properly connected and they have to lead from one control node to another. Moreover navigation points on each ends has to have set boundary lanes from which traffic will come and go to other connected map assets.

If prefab shouldn't have any traffic inside, no navigation point locators should be created.

[[/images/SCS_Tools_Locators_Prefab_NP.png]]

**Low Probability** - property defining smaller visiting probability for AI cars.

**Additive Priority** - property defining that selected value from "Priority Modifier" will be added to already existing priority for this lane.

**Limit Displacement** - property defining extra limited displacement for AI cars.

**Allowed Vehicles** - property defining type of vehicles that are able to enter AI traffic curves starting at this navigation point.

**Blinkers [Left Blinker|No Blinker|No Blinker (forced)|Right Blinker]** - property defining blinker usage for all incoming AI traffic curves connected to this navigation point.

**Priority Modifier** - property defining priority of vehicles driving into the next curve. Priority modifier has to be set only on navigation point which next curve is intersecting with opposite lane or next navigation point is merging more curves. Upon that modifier values game will decide order of cars proceeding in the point of intersection.

> NOTE: if property modifiers won't be properly set game will print out errors about it, so you are able to fix missing priorities.

**Traffic Semaphore** -

**Traffic Rule** -

**Boundary** - 

**Boundary Node** - 


## Map Point

[[/images/SCS_Tools_Locators_Prefab_MP.png]]


## Trigger Point

[[/images/SCS_Tools_Locators_Prefab_TP.png]]