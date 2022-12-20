# Layers and tags

This might change in the future, but due to the way ULTRAKILL was programmed, you have to remember a couple of things.

!> Mark your floors and walls as `Environment` and tag your floors with `Floor`!

![setting the layer and the tag](../_images/setting-layer-and-tag.png)

Additionally, you should mark your walls and floors as Navigation Static if you plan to have enemies there. Only Navigation static objects are included in the [Navmesh bake](navmesh), which is used by enemies.
