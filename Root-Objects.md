SCS Root Objects are special items, which serves as master objects for individual SCS Game Objects (see the chapter “Terminology”). Practically it means, that any object parented to the SCS Root Object automatically belongs to its content and such unit is then called SCS Game Object. It also carries various settings for the whole unit (like Parts and Variants) and can be edited in the SCS Object Specials palette.

You can create a Root Object by adding a Blender's standard “**EMPTY**” object and setting it as “Root Object” in “Object Type” option. You can find this option in Properties window, Object tab, SCS Object Specials within SCS Objects sub-palette.

[[images/SCS_Tools_Root_Object_02.png]]


**Export Inclusion**

With this option you can enable or disable batch export of this SCS Game Object.


**Animated Model / Rigid Model**

If an animated Game object is going to be exported with this switch on “Rigid Model” option, it will be without animation as it was rigid model. And obviously, if game object without animation will be exported with this switch on “Animated Model” option, it will be still rigid.


**Allow Custom Export File Path**

Allow or disable the use of “Custom Export File Path” for this SCS Game Object.


**Custom Export File Path**

Allows to set a custom file path for export of this SCS Game Object (overwrites "Default Export Path").

Specified path must be relative filepath inside "SCS Project Base Path" where this Game Object will be exported.

1. If custom export path is empty, Blender Tools will try to export Game Object beside saved Blender file.
2. If custom export path is set, Blender Tools will combine "SCS Project Base Path" with given custom export path to export files there.

If Blender Tools can't find any solution for cases above, files are exported directly into "SCS Project Base Path".

> NOTE: if input field will be marked red, then path is invalid and extra button for more info will be shown