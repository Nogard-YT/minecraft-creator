---
author: mammerla
ms.author: mikeam
title: Item Documentation - minecraft:on_use_on
ms.prod: gaming
description: "A reference document detailing the 'on_use_on' item component"
---

# Item Documentation - minecraft:on_use_on

`minecraft:on_use_on` allows you to receive an event when the item is used on a block in the world.

>[!IMPORTANT]
> `minecraft:on_use_on` requires the Holiday Creator Features experimental toggle to be set to `true` in order to function properly.
>
>Holiday Creator Features contains experimental gameplay features. As with all experiments, you may see additions, removals, and changes in functionality in Minecraft versions without significant advanced warning.
>
>To learn more about Experimental Features, please visit [Experimental Features in Minecraft: Bedrock Edition](../../../../../Documents/ExperimentalFeaturesToggle.md)

## Parameters

|Name |Default Value  |Type  |Description  |
|:----------|:----------|:----------|:----------|
|on_use_on|*not set*| JSON object| Event trigger for when the item is used.|

## Example

```json
"minecraft:on_use_on":{
    "on_use_on": "minecraft:entity_primed"
}
```
