Export panel is located within Scene tab and offers a quick way for content export to the game.

[[images/SCS_Tools_Export_01.png]]

## Export Modes

### Export Selected

Exports only selected objects, while there are certain logical rules for deciding about objects' inclusion in export from initial selection. When the Root Object is selected, all its content will be exported. When only some mesh objects are selected, then only those are exported for their Game Objects. In these cases it is not important if their Root Object is selected or not.

**Preview Selection** - shows all the objects that will be exported. This is very good way, how to be sure about exported content. It will show always only geometries and locators, that are going to be exported. Selection previewing is extra mode, where you can use ***Numpad*** keys for view manipulation similar way like Blender standardly does – ***4*** and ***6*** keys turn the view left and right, ***8*** and ***2*** keys up and down and ***+*** and ***-*** will zoom in and out. If you press ***Enter*** the export begins and with ***Esc*** key you can cancel the export and get back to the previous selection state.


### Export Scene

Exports all properly set Game Objects in current scene. 
> NOTE: You can specify in each Root Object whether its content has to be exported or not using “Export Inclusion” switch.


### Export All

Exports all properly set Game Objects in all scenes in current Blender file.
> NOTE: You can specify in each Root Object whether its content has to be exported or not using “Export Inclusion” switch.


## Other export options

**Default Export Path** - here you can specify relative filepath inside "SCS Project Base Path" where your Game Objects will be exported. 

1. If default export path is empty, Blender Tools will try to export Game Object beside saved Blender file.
2. If default export path is set, Blender Tools will combine "SCS Project Base Path" with given default export path to export files there.
   
If Blender Tools can't find any solution for cases above, files are exported directly into "SCS Project Base Path".

> NOTE: if input field will be marked red, then path is invalid and extra button for more info will be shown

> NOTE: export path can be overwritten on Root Object by specifying "Custom Export Filepath"


**Scale** - the resulting scale of all exported models and elements. This setting is saved and thus remembered in every Blend file.


**Apply Modifiers** - apply all modifiers before export.


**Apply Only 'Edge Split'** - apply only 'Edge Split' modifier before export to get sharp edges. All the other modifiers will be ignored.

**Output Format** - developers feature only, for now it should be always set to "Game Data Format".
