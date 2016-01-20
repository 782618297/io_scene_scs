Conversion helper panel features tools for automated files conversion and mod packing. Panel with conversion helper can be found below [[Export Panel]] located within Scene tab.

[[images/SCS_Tools_Conv_Hlpr.png]]


### Conversion Tools Path

Property holding path to directory where you extracted [[Conversion Tools]]. Select proper conversion tools depending on the game you want to use your content for.

### Direct Conversion Tools Operators

**CLEAN RSRC** - operator which will immediately clean content that you converted before or is left there from some other time. In general this makes sure your mod won't have any unused resources (leftover textures, old materials) in the converted result.
**CONVERT CURRENT SCS PROJECT** - operator which will only convert resources in your currently set SCS Project Base Path. Use this operator if you want to pack your mod by hand.

### Custom Paths Usage

Custom Paths are holding list property for multiple custom paths you want to convert at the same time. Use this custom paths if you want to merge resources from 2 or more different mods of yours.

On the side of the list you can find operators for managing your custom paths:
* **[[images/SCS_Tools_Conv_Hlpr_Add_Cstm_Path]]** - opens file selector where you should browse for new custom path you want to use.
* **[[images/SCS_Tools_Conv_Hlpr_Del_Cstm_Path]]** - deletes currently selected custom path in the list.
* **[[images/SCS_Tools_Conv_Hlpr_Cstm_Path_Up]]** - moves up currently selected custom path in the list. Ordering in the list doesn't have influence on converted result. It is only there so you can order paths however you like.
* **[[images/SCS_Tools_Conv_Hlpr_Cstm_Path_Down]]** - moves down currently selected custom path in the list. Ordering in the list doesn't have influence on converted result. It is only there so you can order paths however you like.

Under the custom paths list you will also find operator **CONVERT CUSTOM PATHS*** operator which will only convert resources from the custom paths specified in custom paths list. Use this operator if you want to pack your mod later or by hand.


### Mod Packing

This section is featuring properties and operators for packing a mod for SCS game.

**Mod Folder Path** - property holding folder where mod should be placed,
  * ***Mod Name*** - property holding name of the mod ZIP file,
  * ***Auto Clean*** - should be conversion tools previous result be deleted before packing,
  * ***Auto Clean*** - should be ,