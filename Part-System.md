Parts provides a kind of grouping system for Model and Locator objects. It is usually used for defining of Variants (see the chapter “Variant System” below) and also in special cases, when we need to define a part of the geometry, that has to have a different treating then the rest of the model (see the chapter “Predefined Part Names”).

Every object in a scene belongs to some Part. Even in case when we don't need to use Parts, there is always a Part name assigned to every object in a scene. The default name is “defaultpart”, but it can be changed any time. If the active object is not parented to any SCS Root Object, then it is not possible to set the Part name for such object.

[[images/SCS_Tools_Object_Specials_-_Parts_05.png]]


### Part List

Part list is held on every SCS Root Object and it contains all the Part names, which are used within this SCS Game Object.


**Add, Remove, Rename Parts**

You can _**Add**_ or _**Remove**_ names from the Part list using the buttons on the right side of the list. The lowest button here is a _**Remove Unused**_ button, which will automatically remove any unused Part names. To _**Rename**_ the existing Part just double click the item in the list and type a new name.


**Additional List Tools**

There are also some additional tools integrated for each item in Part list and can be used for easy selection/deselection (arrow icon) or hiding/showing (eye icon) of particular Parts. It works like a switches, so if it is pressed repeatedly it will select and deselect or hide and show all the Part items. With _**Shift**_ pressed it will always add to the existing selection or always show the Part items and with _**Ctrl**_ it will always subtract from existing selection or always hide the Part items.


### Item-selection Tools

If the active object is Model, Model Locator or Collision Locator object additional buttons appear.


**Assign**

Assigns currently selected Part name to active object.


**Select**

Select all the Models, Model Locators and Collision Locators within active SCS Game Object which uses the same Part name.


**Deselect**

Deselect all the Models, Model Locators and Collision Locators within active SCS Game Object which uses the same Part name.