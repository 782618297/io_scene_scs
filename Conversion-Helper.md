Conversion helper panel features tools for automated files conversion and mod packing. Panel with conversion helper can be found below [[Export Panel]] located within Scene tab.

> NOTE: Before using this helper make sure you downloaded latest [[Conversion Tools]] for the game you want to create mod for.

[[images/SCS_Tools_Conv_Hlpr.png]]


### Conversion Tools Path

Property holding path to directory where you extracted [[Conversion Tools]]. Select proper conversion tools depending on the game you want to use your content for.

### Direct Conversion Tools Operators

**CLEAN RSRC** - operator which will immediately clean content that you converted before or is left there from some other time. In general this makes sure your mod won't have any unused resources (leftover textures, old materials) in the converted result.

**CONVERT CURRENT SCS PROJECT** - operator which will only convert resources in your currently set SCS Project Base Path. Use this operator if you want to pack your mod by hand.

### Custom Paths Usage

Custom Paths are holding list property for multiple custom paths you want to convert at the same time. Use this custom paths if you want to merge resources from 2 or more different mods of yours.

On the side of the list you can find operators for managing your custom paths:
* **[[images/SCS_Tools_Conv_Hlpr_Add_Cstm_Path.png]]** - opens file selector where you should browse for new custom path you want to use.
* **[[images/SCS_Tools_Conv_Hlpr_Del_Cstm_Path.png]]** - deletes currently selected custom path in the list.
* **[[images/SCS_Tools_Conv_Hlpr_Cstm_Path_Up.png]]** - moves up currently selected custom path in the list. Ordering in the list doesn't have influence on converted result. It is only there so you can order paths however you like.
* **[[images/SCS_Tools_Conv_Hlpr_Cstm_Path_Down.png]]** - moves down currently selected custom path in the list. Ordering in the list doesn't have influence on converted result. It is only there so you can order paths however you like.

Under the custom paths list you will also find operator **CONVERT CUSTOM PATHS** operator which will only convert resources from the custom paths specified in custom paths list. Use this operator if you want to pack your mod later or by hand.


### Mod Packing

This section is featuring properties and operators for packing a mod for SCS game.

First two options are specifying destination and name:
* **Mod Folder Path** - property holding folder where mod should be placed. On the side of this property you have operator ([[images/SCS_Tools_Conv_Hlpr_Find_Folder.png]]) for auto retrieve of the mod paths for Euro Truck Simulator 2 or American Truck Simulator.
* **Mod Name** - property holding name of the mod ZIP file.

Third row is featuring switching of automated actions that should be done before mod will be packed:
* **Auto Clean** - enable this switch if you want to make clean conversion without any leftovers from previous packing or converting.
* **Auto Export** - enable this switch if you want to run automated Blender Tools export. Scope of the content which will be auto exported is defined with Export Scope property in [[Export Panel]].
* **Auto Convert** - enable this switch if you want for your resources to be converted before packing. This automated conversion will convert SCS Project Base Path as well as any defined custom paths.

Last switch **"No Compression | Deflated | BZIP2"** defines type of the compression you want to use for your mod package.

As last there is **PACK CONVERTED DATA** operator which firstly does any selected automated actions and on the end packs conversion tools result into the ZIP package and copies it to the selected mod destination.
