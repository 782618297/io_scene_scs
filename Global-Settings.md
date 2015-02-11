“Global Settings” sub-palette can be find within “SCS Tools” palette in “Scene” settings of the “Properties” window.

[[images/SCS_Tools_Properties_-_icons_01.png]]

There are two sub-palettes: “Path Settings” and “Display Settings”.

[[images/SCS_Tools_Globals_01.png]]


## Path Settings

Before you start to use the tools, it is necessary to specify where to access certain data sources, which are used for filling up of some library menus. First of all, you’ll need to set the main folder that contains your project. Do it to the “SCS Project Path” entry. Other routes usually proceed from that location, and therefore can be stored in the form of a relative path. However that doesn’t need to be the rule every time and therefore the mechanism for path selection in the SCS Tools will always decide the appropriate form for the path. If paths are set properly is clearly seen from color of its background – if any entry is faulty, the background is in red color and needs to be set to the valid location or valid library file.


**SCS Project Base Path** _[folder, always absolute path]_

SCS project's “base” directory. All the paths of following libraries usually continues from this location, so they can be in relative form. However if you prefer another location, you can use it and the path form will be automatically chosen.


**Sign Library** _[“*.sii” file, absolute or relative path to 'SCS Project Base Path']_

Library of predefined traffic Signs. You can assign them to Sign Prefab Locators which are used in game to create traffic signs. These are respected by AI cars and lay the traffic rules for player. Details on Signs you can find in “Signs” chapter.


**Semaphore Library** _[“*.sii” file, absolute or relative path to 'SCS Project Base Path']_

Library of predefined Traffic Semaphore profiles. You can assign them to Traffic Semaphore Prefab Locators which are used in game to create traffic semaphores. These are respected by AI cars and should be respected by player as well. Details on Traffic Semaphores you can find in “Traffic Semaphores” chapter.


**Traffic Rules Library** _[“*.sii” file, absolute or relative path to 'SCS Project Base Path']_

Library of predefined Traffic Rules. You can assign them to Navigation Point Prefab Locators which are used in game to create traffic routes. These are used mainly by AI cars. Details on Traffic Rules you can find in “Navigation Points” chapter.


**Hookup Library** _[folder, absolute or relative path to 'SCS Project Base Path']_

Directory containing predefined Hookup files. You can assign them to Model Locators which are used in game to instance other game models within actual model. Details on Hookups you can find in “Model Locators” chapter.


**Mat Substance Library** _[“*.db” file, absolute or relative path to 'SCS Project Base Path']_

Library of Material Substances, which defines physical behavior of the material. You can assign them to Materials. Details on Substances you can find in “Materials” chapter.


**Shader Presets Library** _[“*.txt” file, absolute file path]_

Shader Presets library filepath. This library has been created specially for SCS Blender Tools and thus it is located in its installation folder. The correct path should be set automatically. Details on Shader Presets you can find in “Materials” chapter.


**Global Export Path** _[folder, absolute path or relative path to saved Blender file]_

Global path for all exported files. If this field is filled with a valid path, all the exported files will be written to this location, otherwise they will be written beside to saved Blender file.
Please note, that this setting can be overridden on SCS Game Object level by Custom Export Path setting on any SCS Root Object (see chapter SCS Root Objects).
If the Blender work wasn't saved yet and this field is empty (as well as Custom Export Path setting on the SCS Root Object), then the Error message is displayed and no export can take place.

`NOTE: Sign, Semaphore, Traffic Rules and Mat Substance libraries are not yet fully supported!`