Prefab locators are used during the creation of prefab map assets. Examples of this assets are: roads, crosses, docking companies, services, gas stations etc. So purpose of prefab locators in this assets is to store data for AI traffic connection/rules, players interactions and GPS navigation. 

Because of different usage and data we have multiple types of Prefab Locators with their own set of properties described below.

## Control Node

Control Node is used: as prefab control in SCS map editor, as connection to other map assets and also as AI traffic entry/exits point. 

For proper prefab creation this requirements have to be meet:
1. Prefab must have from 2 to 6 control nodes;
2. Each control node has to have unique index, defined by "Node Index" property;
3. When creating more than 2 nodes, they have to be placed clockwise starting with index 0;
4. If prefab should be extended with in game generated terrain, then control node has to have terrain points assigned on it's left side.

[[/images/SCS_Tools_Locators_Prefab_CN.png]]

***Node Index*** - saves index of the control node


## Sign

[[/images/SCS_Tools_Locators_Prefab_SIGN.png]]

## Spawn Point

[[/images/SCS_Tools_Locators_Prefab_SP.png]]

## Traffic Semaphore

[[/images/SCS_Tools_Locators_Prefab_TS.png]]

## Navigation Point

[[/images/SCS_Tools_Locators_Prefab_NP.png]]

## Map Point

[[/images/SCS_Tools_Locators_Prefab_MP.png]]

## Trigger Point

[[/images/SCS_Tools_Locators_Prefab_TP.png]]