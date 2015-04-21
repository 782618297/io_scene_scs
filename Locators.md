Locators are used for placing of special items to the “SCS Game Model”.
To create a Locator the first thing you have to do is to create an Empty object (**Shift+A → Empty → \<any type>**).

[[images/SCS_Tools_Locators_01.png]]

Now while the object is active go to the Object Properties tab in Properties window and find “SCS Object Specials” palette. Here is the “SCS Objects” sub-palette, where you can change the Object Type. Change it to Locator type.

[[images/SCS_Tools_Locators_02.png]]

Now you can choose from three types of Locators in the Locator Type drop-down menu: Prefab, Model and Collision.

> NOTE: Prefab and Collision locators are not fully supported yet!


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