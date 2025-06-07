# 🐐 Lc-Eid | Eid al-Adha Script for FiveM

A complete script to celebrate Eid al-Adha within FiveM servers. Includes distributing Eidiya, performing the sacrifice, and utilizing a targeting system compatible with popular systems.

---

## ✨ Features

- 🎁 Distribute Eidiya to players via NPCs.
- 🔪 Sacrifice animals using specified weapons.
- 🔄 Supports three Target systems:
  - `interact`
  - `Lc-target`
  - `ox_target`
- 👤 Fully customizable via `config.lua` file.
- 🐐 Spawn goats/sheep at specified locations.
- 🌍 Ability to set different zones and NPCs.

---

## Installation

qb-core/shared/item.lua
```
['meat_goat'] = {
    ['name'] = 'meat_goat',
    ['label'] = 'Goat Meat',
    ['weight'] = 750,
    ['type'] = 'item',
    ['image'] = 'meat_goat.png',
    ['unique'] = false,
    ['useable'] = false,
    ['shouldClose'] = false,
    ['combinable'] = nil,
    ['description'] = 'Fresh goat meat, perfect for Eid!'
},
```
