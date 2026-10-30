<img align="center" src="./src/main/resources/icon.png">
<h1 align="center">salmonberries</h1>
<p align="center">Keep your items after you die.</p>


_Inspired by PuckiSilver's [Keep Some Inventory](https://modrinth.com/datapack/keep-some-inventory) datapack._

**Keep Some Modded Inventory** is an alternative to Minecraft's `keepInventory`: you can keep your equipment (swords, pickaxes, etc.), but your other items (food, torches, etc.) will drop on death. This means it is much easier to get back to your stuff, but dying still has a penalty. Additionally, it has some small QoL features to make dying less of a chore.

## Features

_By default..._
- Vanilla and modded equipment will stay in your inventory when you die.
- Your resources will drop **exactly** where you died, with no splattering.
- Your items will **never** despawn.
- **100%** of your experience will drop

_Additonally..._
- This mod uses dynamic predicates to decide whether an item should be dropped or not, meaning that it is automatically compatable with most modded tools and weapons.
- Compatabile with most gravestone mods.
- Compatabile with [Accessories](https://modrinth.com/mod/accessories).
- Compatabile with [YYZ's Backpack](https://modrinth.com/mod/yyzs-backpack) and [Sophisticated Backpacks](https://modrinth.com/mod/sophisticated-backpacks) (backpacks will drop on death to prevent circumventing KSMI)
- Fully configurable!

## Configuring
This mod can be configured in the mod menu, as well as with datapacks.
<details>
  <summary>Configuration properties</summary>

  | Property                 | Description                 | Default |
  |--------------------------|-----------------------------|---------|
  | Mod enabled              | Whether the mod is enabled. | true    |
  | Keep enchantable items   | When true, enchantable items not in the `always_drop` tag will be kept in inventory. | true |
  | Keep damageable items    | When true, items with the `max_damage` component not in the `always_drop` tag will be kept in inventory. | true |
  | Keep equippable items    | When true, items that can be equipped as armor or as an [accessory](https://modrinth.com/mod/accessories) not in the `always_drop` tag will be kept in inventory. | true |
  | Item velocity multiplier | How much items should be flung when you die. 1 is vanilla's default. | 0.1 |
  | Experience dropped       | Percent of experience should be dropped when you die. Set to 0 to use Minecraft's calculations. | 1.0 |
  | Despawn time             | Time in minutes that items dropped on death should last. Set to 0 to make them never despawn. | 0 |
  
</details>
<details>
  <summary>Datapack configuration</summary>

  Datapacks can be used to have full control over what items drop on death. KSMI 
  provides two item tags: `#keepsomemoddedinventory:never_drop` and `#keepsomemoddedinventory:always_drop`. These tags take precidence over the predicates in the config. By default, tool items like the spyglass or compass are in the `#never_drop` tag and container items like the shulker box are in the `#always_drop` tag.
</details>

