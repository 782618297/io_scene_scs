Model Locators can be used to place an existing game models to other game model without the need to include their data physically in host file. Simply said, these models are only referenced in the host file. This way you can for example define a places in a truck model, where mirrors or other upgrades will appear in the game by player's will.

[[images/SCS_Tools_Locators_-_Model_02.png]]


**Name**

This property here is the same as Blender Object's name and will be used by game engine (e. g. in the model of wheels for ETS2, "bb" is the name of the locator which represents size of the wheel).

**Hookup**

This property can be set according to records in “Hookup Library” (see the chapter “Path Settings” in [[Global Settings]]). However hookup property is used to bind other game objects to the current. Examples of hookups are: flares for lights, pedestrian spawning on prefabs, company logos on prefabs etc.

> NOTE: Model Locators can also use "Preview Model" feature (see the chapter “Preview Models”).