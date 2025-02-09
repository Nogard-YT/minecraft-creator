---
author: mammerla
ms.author: mikeam
title: Item Documentation - minecraft:weapon
ms.prod: gaming
description: "A reference document detailing the 'weapon' item component"
---

# Item Documentation - minecraft:weapon

`minecraft:weapon` sets the weapon item component. Added to every weapon item such as axe, sword, trident, bow, and crossbow.

>[!IMPORTANT]
> `minecraft:weapon` requires the Holiday Creator Features experimental toggle to be set to `true` in order to function properly.
>
>Holiday Creator Features contains experimental gameplay features. As with all experiments, you may see additions, removals, and changes in functionality in Minecraft versions without significant advanced warning.
>
>To learn more about Experimental Features, please visit [Experimental Features in Minecraft: Bedrock Edition](../../../../../Documents/ExperimentalFeaturesToggle.md)

## Parameters

|Name |Default Value  |Type  |Description  |
|:----------|:----------|:----------|:----------|
|on_hit_block|*not set*| String|Trigger for letting you know when this item is used to hit a block|
|on_hurt_entity|*not set*| String|Trigger for letting you know when this item is used to hurt another mob|
|on_not_hurt_entity|*not set*| String|Trigger for letting you know when this item hit another actor, but didn't do damage|

## Example

```json
"minecraft:weapon":{
    "on_hit_block" : "minecraft:block_hit", //custom event
    "on_hurt_entity" : "minecraft:ouch", //custom event
    "on_not_hurt_entity" : "minecraft:panic", //custom event
}
```
