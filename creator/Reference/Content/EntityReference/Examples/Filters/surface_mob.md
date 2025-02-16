---
author: mammerla
ms.author: mikeam
title: Entity Documentation - surface_mob
ms.prod: gaming
description: "A reference document detailing the 'surface_mob' entity filter"
---

# Entity Documentation - surface_mob

Tests if the subject is a surface mob.

## Parameters

> [!NOTE]
> `surface_mob` does **not** require any parameters to work properly. It can be used as a standalone filter.
>
> `surface_mob` can also use `subject`, [operator](../Definitions/NestedTables/operator.md) and `value` parameters.

### subject

| Options| Description |
|:-----------|:-----------|
| block| The block involved with the interaction. |
| damager| The damaging entity involved with the interaction. |
| other| The other member of an interaction, not the caller. |
| parent| The caller's current parent. |
| player| The player involved with the interaction. |
| self| The entity or object calling the test |
| target| The caller's current target. |

### operator

| Options| Description |
|:-----------|:-----------|
| !=| Test for inequality. |
| <| Test for less-than the value. |
| <=| Test for less-than or equal to the value. |
| <>| Test for inequality. |
| =| Test for equality. |
| ==| Test for equality. |
| >| Test for greater-than the value. |
| >=| Test for greater-than or equal to the value. |
| equals| Test for equality. |
| not| Test for inequality. |

### value

|Name |Default Value  |Type  |Description  |
|---------|---------|---------|---------|
|value |true |Boolean |(Optional) true or false. |

## Examples

### Full

```json
{ "test": "surface_mob", "subject": "self", "operator": "equals", "value": true}
```

### Short (using Defaults)

```json
{ "test": "surface_mob" }
```

## Vanilla entities examples

No entities currently use `surface_mob`.

## Vanilla entities using `surface_mob`

No entities currently use `surface_mob`.
