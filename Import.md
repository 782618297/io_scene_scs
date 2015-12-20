You can import models and other elements which were exported to _SCS mid-format_ data. All these files uses ***PIX*** file extensions. ***PIM*** files are considered as main files containing model geometries, other extensions are ***PIT*** (trait data), ***PIC*** (colliders data), ***PIP*** (prefab data), ***PIS*** (skeleton data) and ***PIA*** (animation data).

[[images/SCS_Tools_Import_01.png]]

The import functionality is in _Blender's_ import menu as “_SCS Formats (.pim)_”. Within the file requester you can find “_SCS Import_” panel.

## Import Options

[[images/SCS_Tools_Import_02.png]]

**Scale** - scale of imported meshes and other elements.

**Import Model (PIM)** - you can turn _Model_ file loading **ON** and **OFF**.

**Use Normals** - if this property is ticked, mesh will be imported with normals written in file. Otherwise normals are recalculated by Blender itself.

**Use Welding** - if this property is ticked, automatic vertex welding operation is performed on all imported meshes. It is sometimes necessary, because mesh geometries in ***PIX*** files are exported in a form, which can be called like “graphics-card-friendly”. It means, that vertices are doubled in many cases – on all places where hard edges are, UVs are not continuous, vertex colors are different for neighboring faces, etc. Auto Welding tries to make geometries as compact as possible.

> NOTE: This feature can be time-consuming on larger geometries.

**Welding Precision** - threshold in decimal numbers to which values has to be the same that welding can take place. So in case of default value 4, values have to match up to for decimals which is in millimetre measurement 0.1 mm.

**Import Trait (PIT)** - you can turn _Trait_ file loading ***ON*** and ***OFF***.

**Load Textures** - if this property is ticked, all image textures will be loaded.

**Import Collision (PIC)** - you can turn _Collision_ file loading ***ON*** and ***OFF***.

**Import Prefab (PIP)** - you can turn _Prefab_ file loading ***ON*** and ***OFF***.

**Import Skeleton (PIS)** - you can turn _Skeleton_ file loading ***ON*** and ***OFF***.

**Bone Scale** - here you can specify the size of imported bones. It is usually rather complicated to change their size later.

**Import Animations (PIA)** - you can turn _Animation files_ loading ***ON*** and ***OFF***.

**Search Subdirectories** - if this property is ticked, all available subdirectories will be searched for animation files.
> NOTE: Only animation files which belongs to an actual skeleton can be loaded. If they are not placed beside PIX files or any subdirectory, then you can still import animations later from [SCS Animations Panel](Animation-System#scs-animations-panel)