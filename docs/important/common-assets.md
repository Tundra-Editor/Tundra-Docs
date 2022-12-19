# Common Assets

Common assets are assets that ship with ULTRAKILL. They don't get bundled with your map, and get referenced instead, keeping the size of your map low.

## Important Warning

:::danger

Do **not** modify common assets!

:::

It's best to pretend that everything inside of `Common` folder is read-only, as that's how it'll be treated by the exporter.

## Properly Modifying Common Assets

If you want to modify any common assets, such as textures or prefabs, you should **copy** them outside of the Common folder first.

You might have to update references to the copied assets.

For example, if you copy both a material and a texture, you will have to update the **copied** material to use the **copied** texture instead of the **original** one if you plan on editing it as well.

## Terminology

:::note

Common Assets are sometimes referred to as **Magenta**.

:::
