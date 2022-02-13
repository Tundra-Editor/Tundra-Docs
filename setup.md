# Setup

There are couple of things that you have to do before making your map.

## Map Info

!> If you made a map via the `Quick New Map` feature, an object with Map Info should already exist.

Every Tundra map needs a Map Info component.

The best way to go about it is to create a new empty GameObject and add MapInfo to it.

![create empty](_images/creating-map-info.png)

That should leave you with a mostly Map Info component.
Next, click the `Generate an Id` button and fill in the rest of the details. You can leave the thumbnail empty for now.

![empty map info component](_images/empty-map-info-component.png)

![filled map info component](_images/filled-map-info-component.png)

## First Room

Auto prefabs or placeholder prefabs are special. You can **not** modify them because the game will replace them with the actual functional version.

The First Room and its variations are the most important placeholder prefabs. Drag either one into your scene, and preferably make sure that its position is set to 0, 0, 0.

![first room prefabs](_images/first-room-prefabs.png)

![first room comparison](_images/first-room-comparison.png)

The secret variant doesn't have a shop, meaning the player cannot modify their loadout.

FirstRoom Secret has a **PlayerLoadout** component, use it to forcefully enable or disable certain or all weapons.

![custom loadout](_images/custom-loadout.png)

## Stats Manager

StatsManager is the second prefab required to make your map functional. Drag and drop it into your scene as well.

![stats manager prefab](_images/stats-manager-prefab.png)

You can modify it or its children to change some things about your map, such as the music.

!> **Don't** apply the prefab overrides! Keep the changes in the scene file instead of the shared StatsManager file.
