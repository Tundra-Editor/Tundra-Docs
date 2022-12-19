# Prefabs

## Different types of prefabs

Tundra comes with two types of prefabs:

- **Auto Prefabs** are prefabs that don't get baked into your maps, and so they cannot be modified beyond the top-level components.
- **Normal Prefabs** are just standard prefabs that can be fully modified.

Some prefabs come in both variants, and others only have one.

## Usage

In general, auto prefabs should be preferred over normal prefabs.

Using them keeps your maps smaller and less prone to breaking with updates.

Use normal prefabs over auto prefabs only if you want to modify the prefab.

## Saving Modified Prefabs

As long as you keep all of your changes as scene [Prefab Overrides](https://docs.unity3d.com/Manual/PrefabInstanceOverrides.html), you don't have to worry about anything.

:::tip

If you do want to apply your overrides, please read [Common Assets](common-assets) first.

:::
