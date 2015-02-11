
**SCS Root Object**

It is Blender “**EMPTY**” Object with appropriate setting in SCS Tools. It works as a root object and anything parented to it will become its content. It also carries set of settings for the whole such entity, that can be exported in a result as a “SCS Game Object” (see the chapter “SCS Game Object” below). For more details on “SCS Root Object” see the chapter “SCS Root Objects”.


**SCS Game Object**

This is a general term for a unit, which consists of properly set “SCS Root Object” and its valid content. If one or more components from this entity are for any reason considered invalid during export, the user is informed about it in console and these items are automatically skipped. If all components are invalid, the entire “SCS Game Object” gets skipped.


**Model**

By the term “Model” we simply mean any Blender object of **MESH** type.


**Locator**

“Locators” we call any Blender object of **EMPTY** type, which is set as Locator in SCS Blender Tools.

TODO: INSERT IMAGE

There are three types of Locators:

1. **Model Locator** - can be used to place (reference) existing game model. Details on Model Locators you can find in [“Model Locators”](URL) chapter.
2. **Prefab Locator** - can be used to create various types of special items for use in prefab models. Details on Prefab Locators you can find in [“Prefab Locators”](URL) chapter.
3. **Collision Locator** - can be used to create several types of collision envelopes for physical interaction of bodies in the game. Details on Collision Locators you can find in [“Collision Locators”](URL) chapter.