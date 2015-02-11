Variants are groups of Parts, which allows to set up a different variations of a game model. For example a truck model in its multiple variations, where different Variants can use different cabins, chassis or spoilers. Variants provide a sufficient way how to set these “truck versions” in any combinations of the Parts.

If you want to set Variants in your game model, you have to set some Parts and create a SCS Root Object (see the chapter “Terminology” or “SCS Tools Shelf > Add Root”). Then select SCS Root Object and go to Properties window into Object tab and in “SCS Object Specials” palette you'll find the “SCS Variant” sub-palette. Here you can find all the settings and tools for work with Variants.

[[images/SCS_Tools_Object_Specials_-_Variants_05.png]]


### Variant List

List of Variants can contain no Variant. The palette has buttons on right side for adding and removing items. You can also double-click on any item in the list to rename it.

If there is at least one Variant created, an “Variant-Part Table” is displayed under the list (or directly within the list in case of Integrated view style; see below). This “Variant-Part Table” always include complete list of all Parts, which are collected from all objects in current “SCS Game Object”. Here any Part can be turned ON or OFF for an individual Variant.

The Variant list uses the standard Blender list mechanism, so you can use all the advantages of this system – filtering of items and custom sorting. Just click a small plus [+] icon in lower left corner of the list to make these available.


**Additional List Tools**

There are also an additional tools integrated for each item in Variant list and can be used for easy selection/deselection (arrow icon) or hiding/showing (eye icon) of particular Variants. It works like a switches, so if it is pressed repeatedly it will select and deselect or hide and show all the Variant items. With _**Shift**_ pressed it will always add to the existing selection or always show the Variant items and with _**Ctrl**_ it will always subtract from existing selection or always hide the Variant items.


### View Styles

You can choose among four view styles for the “Variant-Part Table”: Compact, Vertical, Horizontal and Integrated. The default one is Horizontal view style.


**Compact View Style**

[[images/SCS_Tools_Object_Specials_-_Variants_07.png]]

The only active Variant in the list is displayed. This style is good if you have any amount of Parts and Variants and you'd like to view and edit a single Variant at a time.

You can change display order of Parts from unsorted (the order in which the items were created) to alphabetical using Part alphabetical sorting button.


**Vertical View Style**

[[images/SCS_Tools_Object_Specials_-_Variants_08.png]]

All the Variants are displayed vertically in a column. This style is good if you have large amount of Variants and you'd like to go through them one after the other.

You can change display order of Parts and/or Variants from unsorted (the order in which the items were created) to alphabetical using Part or Variants alphabetical sorting buttons respectively.


**Horizontal View Style**

[[images/SCS_Tools_Object_Specials_-_Variants_06.png]]

All the Variants are displayed horizontally in a row with all its Parts in columns. This style is good if you have rather smaller amount of Variants and you'd like to view and edit them in a well-arranged table-like form.

You can change display order of Parts and/or Variants from unsorted (the order in which the items were created) to alphabetical using Part or Variants alphabetical sorting buttons respectively.


**Integrated View Style**

[[images/SCS_Tools_Object_Specials_-_Variants_09.png]]

In this view style there is no “Variant-Part Table” special area where all the Parts are exposed, but instead they are displayed directly within the Variant list. This style can be beneficial if you have small amount of Parts and you'd like to view and edit them in a well-arranged table-like form with no additional UI clutter.

The Additional List Tools (see above) are in this case exposed just under the list box and they have effect always on selected item in the list.