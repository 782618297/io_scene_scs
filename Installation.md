Before installation make sure you have downloaded SCS Blender Tools from the [[Download]] page or via cloning GIT repository.

### 1. Copying Files
All the files needed for tools installation are contained in a single folder named "addon/io_scs_tools". This folder must be placed in a location, where Blender can find it and read it as an Addon. It is possible to use an installation method, where you can just point Blender to the Addon location (e.g. if you want to run the tools right from GIT repository).

You can use one the following installation possibilities:

1. **LOCAL INSTALLATION:** Place the folder "addon/io_scs_tools" to your installation of Blender to the location "\<Blender_installation>/\<version_number>/scripts/addons/". The Addon will be used only by this particular installation of Blender.
2. **GLOBAL INSTALLATION:** Place the folder "addon/io_scs_tools" in your profile to the location "\<user_profile>/blender/\<version_number>/scripts/addons/". Addon will be used by any Blender installation of specified version.
3. **INSTALLATION TO THE USER DIRECTORY:** In "User Preferences" within "File" section is the "Scripts" item where you can set the path to any Addon location. This way, for example, you can use any Addon directly from data repository and your tools will always be of the current version in all of your Blender installations. It is necessary for the Addon folder to be placed inside a folder named "addons_contrib" and Blender needs to be directed to its parent folder. Therefore the resulting path to the folder Addons should look like "/\<folder>/addons_contrib/io_scs_tools", but the path under Scripts will be only "/\<folder>".
[[images/Blender_custom_location_for_Scripts.png]]
4. **INSTALL FROM FILE:** Tools can also be installed using the "Install from File..." button, which you can find in "User Preferences" in the "Addons" section on the bottom bar.

### 2. Addon Activation
Now it is necessary to activate the "SCS Blender Tools" Addon. This can be easily done in the "User Preferences" in the "Addons" section. In the upper left part of the window click on "Testing" button and in the main window, look for the "Import-Export: SCS Tools". You can use search feature to locate the item. Now activate the checkbox on the right side of SCS Tools entry. If the item is missing in your list, press F8 to reload Addons.

[[images/Blender_enable_SCS_Tools_Addon.png]]

> NOTE: In order to actually use content in SCS games you also need to install and use conversion tool for specific game. More info about conversion tools: [[Conversion Tools]]