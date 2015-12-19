Global Settings hold common settings to whole SCS Blender Tools addon and are defined per-machine not per-blender file like any other properties in Blender.

> NOTE: Altered items are written to the settings file (config.txt) immediately, so the next time you start Blender all the settings will be preserved, even if application experience crash. If you want to reset settings to default navigate to installed Blender Tools in file browser, delete file "io_scs_tools/config.txt" and restart Blender.

***Global Settings*** sub-palette can be find within ***SCS Tools*** palette in ***Scene*** settings of the Properties window.

[[images/SCS_Tools_Properties_-_icons_01.png]]

There are two sub-palettes: ***Path Settings*** and ***Display Settings***.

[[images/SCS_Tools_Globals_01.png]]


## Path Settings

Before you start to use the tools, it is necessary to specify where to access data sources, which are used for filling up of some library menus and addressing textures. First of all, you’ll need to set the main folder that contains your project. Do it to the “SCS Project Base Path” entry. Other routes usually proceed from that location, and therefore can be stored in the form of a relative path. However that doesn’t need to be the rule every time and therefore the mechanism for path selection in the SCS Tools will always decide the appropriate form for the path. If paths are set properly is clearly seen from color of its background – if any entry is faulty, the background is in red color and needs to be set to the valid location or valid library file.

[[images/SCS_Tools_Globals_Path_01.png]]


**SCS Project Base Path** _[folder, always absolute path]_

***This is most important path, which leads to “base” directory of any SCS game. Base directory always has to have specific structure, because of relative texture and definition file addressing.*** So all of the paths of following libraries should continue from this location and should be in relative form. However if you prefer another location for those libraries, you can use it and the path form will be automatically chosen.

> NOTE: For importing sample models make sure you set SCS Project Base Path to one of the sample base folders inside "data" directory of downloaded SCS Blender Tools package.

> NOTE: You should prefer another location for libraries only if you are using any custom library file.

**Trigger Action Library** _[“*.sii” file, absolute or relative path to 'SCS Project Base Path']_

Library of predefined trigger actions. You can assign them to Trigger Prefab Locators which are used in game for triggering various actions (for example sleeping areas).


**Sign Library** _[“*.sii” file, absolute or relative path to 'SCS Project Base Path']_

Library of predefined traffic Signs. You can assign them to Sign Prefab Locators which are used in game to create traffic signs or any model defined as sign. Most of them are respected by AI cars and lay the traffic rules for player. Details on Signs you can find in “Signs” chapter.


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


## Display Settings

The “Display Settings” sub-palette brings together visual settings for all the special elements that are part of SCS Blender Tools. You can find here a visual settings for Locators, their Curves, Preview Models and other specific elements, which detail explanation follows in the text below.

[[images/SCS_Tools_Globals_Display.png]]


**Drawing Mode**

Drawing mode for custom elements (i.e. Locators and Connections). It switches between Normal and X-Ray mode. Normal mode use normal depth testing drawing so all the custom elements are drawn within the scene the same way as the other objects, while the X-Ray mode use X-Ray drawing making all the custom elements visible on top of the other objects.


**Display Locators**

Turns on and off displaying of custom representation of Locators. This can be useful especially when tunning Navigation curves.


**Locator Size**

Drawing size of Locators' custom representation.


**Locator Empty Object Size**

Drawing size ratio of selectable Empty objects in Locators. Alter it if you experience difficulties with selecting of Locators.


**Prefab Locator Color**

Custom color for Prefab Locators.


**Model Locator Color**

Custom color for Model Locators.


**Collider Locator Wire Color**

Custom color for Collider Locators' wire frames.


**Collider Locator Face Color**

Custom color for Collider Locators' faces.


**Display Connections**

Turns on and off displaying of Locators' connections - Curves and Lines.


**Optimized Connections Draw**

Draw connections only when data are updated. Switching this off might give you FPS (frames per second), especially on heavy Prefab scenes.


**Curve Segments**

Number of segments for Navigation Curves. It can improve update speed of 3D View.


**Navigation Curve Base Color**

Custom color for Navigation Curves.


**Map Line Base Color**

Custom color for Map Lines.


**Trigger Line Base Color**

Custom color for Trigger Lines.


**Display Text Info**

Switches displaying of different additional information texts for Locators directly in 3D View. This is very useful when you work on Prefab models. For example, you can display only the Locator Names, or Boundary Lanes or Nodes.


**Info Text Color**

Custom color for Info Texts.


**Show Preview Models**

Turns on and off displaying of Preview models for Locators.