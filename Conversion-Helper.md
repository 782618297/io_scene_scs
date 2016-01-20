Conversion helper panel features tools for automated files conversion and mod packing. Panel with conversion helper can be found below [[Export Panel]] located within Scene tab.

[[images/SCS_Tools_Conversion_Helper.png]]

* ***Conversion Tools Path*** - property holding path to directory where you extracted [[Conversion Tools]]. Select proper conversion tools depending on the game you want to use your content for.
* ***CLEAN RSRC*** - operator which will immediately clean content that you converted before or is left there from some other time. In general this makes sure your mod won't have any unused resources (leftover textures, old materials) in the converted result.
* ***CONVERT CURRENT SCS PROJECT*** - operator which will only convert resources in your currently set SCS Project Base Path. Use this operator if you want to pack your mod by hand,
* ***Custom Paths*** - list property holding multiple custom paths you want to convert at the same time. Use this custom paths if you want to merge resources from 2 or more different mods of yours,
* ***CONVERT CUSTOM PATHS*** - operator which will only convert resources from the custom paths specified in ***Custom Paths*** list. Use this operator if you want to pack your mod by hand,
* ***Mod Packing*** - section featuring properties and operators for packing a mod from a conversion result:
  * ***Mod Folder Path*** - property holding folder where mod should be placed,
  * ***Mod Name*** - property holding name of the mod ZIP file,
  * ***Auto Clean*** - should be conversion tools previous result be deleted first,