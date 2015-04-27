Almost all shaders inside SCS Game engine are using vertex colors. That's why it's very important how you set them. If shader explicitly doesn't specify otherwise then vertex colors with values 0.5 are actually neutral colors and won't change the look of resulting mesh inside game. If vertex colors are below 0.5 it will "darken" the model and what will be above 0.5 will result in "brighter" mesh. 

In addition to this there is Wrap Tool which helps you wrap vertex colors of active vertex color layer on specified interval. So if you baked or painted your model on the range from 0 to 1 you can easily use this tools to scale this interval to the one you define in operator properties (advised interval is from 0.4 to 0.6). Tool can be found in SCS Tools shelf if current object is in "Vertex Paint" mode.

[[images/SCS_Tools_Shelf_-_Wrap_Tool.png]]

* **Wrap All** - wrap vertex colors on all vertices
* **Wrap Selected** - wrap vertex colors only on selected vertices