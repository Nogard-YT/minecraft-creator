---
author: mammerla
ms.author: mikeam
title: Particle Documentation - Emitter Rate Instant component
ms.prod: gaming
description: "A reference document detailing the 'emitter rate instant' particle component"
---

# Particle Documentation - Emitter Rate Instant component

All particles come out at once, then no more unless the emitter loops.

```json
"minecraft:emitter_rate_instant": {
    // this many particles are emitted at once
    // evaluated once per particle emitter loop
    "num_particles": <float/molang> <default:10>
}
```
