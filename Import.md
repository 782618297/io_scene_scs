You can import models and other elements which were exported to _SCS mid-format_ data. All these files uses **PIx** file extensions. **PIM** files are considered as main files containing model geometries, other extensions are **PIT** (trait data), **PIC** (colliders data), **PIP** (prefab data), **PIS** (skeleton data) and **PIA** (animation data).

[[images/SCS_Tools_Import_01.png]]

The import functionality is in _Blender's_ import menu as “_SCS Formats (.pim)_”. Within the file requester you can find “_SCS Import_” panel.

### Import Panel

[[images/SCS_Tools_Import_02.png]]

“_Scale_” – scale of imported meshes and other elements.

“_Import Model (PIM)_” – you can turn _Model_ file loading **ON** and **OFF**.

“_Auto Welding_” – if this checkbox is ticked, automatic vertex welding operation is performed on all imported meshes. It is sometimes necessary, because mesh geometries in **PIx** files are exported in a form, which can be called like “graphics-card-friendly”. It means, that vertices are doubled in many cases – on all places where hard edges are, UVs are not continuous, vertex colors are different for neighboring faces, etc. _Auto Welding_ tries to make geometries as compact as possible.
> NOTE: This feature can be time-consuming on larger geometries.

“_Import Trait (PIT)_” – you can turn _Trait_ file loading **ON** and **OFF**.

“_Load Textures_” – if this checkbox is ticked, all image textures will be loaded.

“_Import Collision (PIC)_” – you can turn _Collision_ file loading **ON** and **OFF**.

“_Import Prefab (PIP)_” – you can turn _Prefab_ file loading **ON** and **OFF**.

“_Import Skeleton (PIS)_” – you can turn _Skeleton_ file loading **ON** and **OFF**.

“_Bone Scale_” – here you can specify the size of imported bones. It is usually rather complicated to change their size later.

“_Import Animations (PIA)_” – you can turn _Animation files_ loading **ON** and **OFF**.

“_Search Subdirectories_” – if this checkbox is ticked, all available subdirectories will be searched for animation files.
> NOTE: Please note, that only animation files which belongs to an actual skeleton can be loaded.