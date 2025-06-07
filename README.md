# 🐐 Lc-Eid | AboMalak

سكربت متكامل للاحتفال بعيد الأضحى داخل خوادم FiveM. يشمل توزيع العيدية، أداء الأضحية، واستخدام نظام استهداف متوافق مع أشهر الأنظمة.

---

### ✅ المتطلبات الأساسية

- QB-Core (https://github.com/qbcore-framework/qb-core)
- qb-inventory (https://github.com/qbcore-framework/qb-inventory)
---

## ✨ الميزات

- 🎁 توزيع العيدية للاعبين من خلال NPC.
- 🔪 ذبح الحيوانات باستخدام أسلحة مخصصة.
- 🔄 يدعم 4 أنظمة Target:
  - [interact](https://github.com/darktrovx/interact)
  - [Lc-target](https://github.com/Lc-Scripts/Lc-target)
  - [qb-target](https://github.com/qbcore-framework/qb-target)
  - [ox_target](https://github.com/overextended/ox_target)
- ⚙️ قابل للتخصيص بالكامل عبر ملف `config.lua`.

---

## ⚙️ التثبيت

### 1. إضافة العناصر إلى `qb-core`

افتح الملف التالي:

```
qb-core/shared/items.lua
```

وأضف ما يلي داخل جدول العناصر:
```
['meat_goat'] = {
    ['name'] = 'meat_goat',
    ['label'] = 'Goat Meat',
    ['weight'] = 750,
    ['type'] = 'item',
    ['image'] = 'meat_pig.png',
    ['unique'] = false,
    ['useable'] = false,
    ['shouldClose'] = false,
    ['combinable'] = nil,
    ['description'] = 'Fresh goat meat, perfect for the holiday!'
},

['cake'] = {
    ['name'] = 'cake Eid',
    ['label'] = 'cake Eid',
    ['weight'] = 1,
    ["created"] = nil,
    ["decay"] = 10.0,
    ["isDecay"] = true,
    ['type'] = 'item',
    ['image'] = 'cake.png',
    ['unique'] = false,
    ['useable'] = true,
    ['shouldClose'] = true,
    ['combinable'] = nil,
    ['description'] = 'cake Eid'
},
```

### 2. اضافة الصور ل`inventory/html/images/`

افتح الانفينتوري وضيف صور الايتمات:

```
inventory/html/images/
```
```
meat_pig.png
cake.png
```

---
## ✅ ملاحظات

- تأكد من وجود الصور (`meat_goat.png`, `pancakes.png`) في مجلد الصور الخاص الانفينتوري.
- يجب على اللاعبين امتلاك أسلحة محددة لذبح الخروف ( `weapon_knife`، `weapon_machete`).
- يمكنك اختيار نظام Target المفضل لديك من خلال `Config.TargetSystem` في ملف `config.lua`.

---

## 📌 المطور

- Developed by: **AboMalak**
- Discord Support: **https://discord.gg/LcStore | https://discord.gg/kYKWhyM2D4**

---

## 📜 ترخيص

لا يجوز بيع أو إعادة توزيع هذا السكربت دون إذن صريح


---

# 🐐 Lc-Eid | AboMalak

A complete script to celebrate Eid al-Adha inside FiveM servers. Includes giving Eidiya, sacrificing animals, and utilizing a targeting system compatible with popular systems.

---

## ✅ Requirements

- QB-Core (https://github.com/qbcore-framework/qb-core)
- qb-inventory (https://github.com/qbcore-framework/qb-inventory)

## ✨ Features

- 🎁 Distribute Eidiya to players via NPCs.
- 🔪 Sacrifice animals using specific weapons.
- 🔄 Supports 4 targeting systems:
  - [interact](https://github.com/JacobWilliams/interact)
  - [Lc-target](https://github.com/Lc-Scripts/Lc-target)
  - [qb-target](https://github.com/qbcore-framework/qb-target)
  - [ox_target](https://github.com/overextended/ox_target)
- ⚙️ Fully customizable via `config.lua`.

---

## ⚙️ Installation

### 1. Add items to `qb-core/shared/items.lua`

Open the following file:
```
['meat_goat'] = {
    ['name'] = 'meat_goat',
    ['label'] = 'Goat Meat',
    ['weight'] = 750,
    ['type'] = 'item',
    ['image'] = 'meat_pig.png',
    ['unique'] = false,
    ['useable'] = false,
    ['shouldClose'] = false,
    ['combinable'] = nil,
    ['description'] = 'Fresh goat meat, perfect for the holiday!'
},

['pancakes'] = {
    ['name'] = 'pancakes',
    ['label'] = 'Pancakes',
    ['weight'] = 1,
    ["created"] = nil,
    ["decay"] = 10.0,
    ["isDecay"] = true,
    ['type'] = 'item',
    ['image'] = 'pancakes.png',
    ['unique'] = false,
    ['useable'] = true,
    ['shouldClose'] = true,
    ['combinable'] = nil,
    ['description'] = 'pancakes'
},
```

### 2. Add images to `inventory/html/images/`

Open the following folder:

```
inventory/html/images/
```
---

## ✅ Notes

- Ensure the images (`meat_goat.png`, `pancakes.png`) exist in your inventory's image folder.
- Players must have specific weapons to sacrifice the animal (e.g., `weapon_knife`, `weapon_machete`).
- You can select your preferred Target system via `Config.TargetSystem` in `config.lua`.

---

## 📌 Developer

- Developed by: **AboMalak**
- Discord Support: **https://discord.gg/LcStore | https://discord.gg/kYKWhyM2D4**

---

## 📄 License

This script may not be sold or redistributed without explicit permission.


## Images

![meat_goat.png](https://cdn.discordapp.com/attachments/1057493068439359549/1380747013448142950/meat_pig.png?ex=6845005d&is=6843aedd&hm=5c866582bad364c1542224d9f5c5e126375d8af270a6636424c7185eac4d768e&)
![cake.png](https://cdn.discordapp.com/attachments/1057493068439359549/1380747966939398185/cake.png?ex=68450140&is=6843afc0&hm=4eaea7b41fe259426c6c8faca9ac37ece7198919309bbc812bc4068704f395a7&)
