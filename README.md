# 🐐 Lc-Eid | AboMalak

سكربت متكامل للاحتفال بعيد الأضحى داخل خوادم FiveM. يشمل توزيع العيدية، أداء الأضحية، واستخدام نظام استهداف متوافق مع أشهر الأنظمة.

---

## ✨ الميزات

- 🎁 توزيع العيدية للاعبين من خلال NPC.
- 🔪 ذبح الحيوانات باستخدام أسلحة مخصصة.
- 🔄 يدعم 4 أنظمة Target:
  - [interact](https://github.com/darktrovx/interact)
  - [Lc-target](https://github.com/Lc-Scripts/Lc-target)
  - [qb-target](https://github.com/qbcore-framework/qb-target)
  - [ox_target](https://github.com/overextended/ox_target)
- 🐐 ظهور الخراف أو الماعز في مواقع مخصصة.
- 🌍 إمكانية تحديد مناطق و NPCs مختلفة حسب الرغبة.
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
    ['image'] = 'meat_goat.png',
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

---
## ✅ ملاحظات

- تأكد من وجود الصور (`meat_goat.png`, `pancakes.png`) في مجلد الصور الخاص بمخزنك.
- يجب على اللاعبين امتلاك أسلحة محددة لذبح الحيوان (على سبيل المثال `weapon_knife`، `weapon_machete`).
- يمكنك اختيار نظام الهدف المفضل لديك من خلال `Config.TargetSystem` في ملف `config.lua`.

---

## 📌 Developer

- Developed by: **AboMalak | LcStore**
- Discord Support: **https://discord.gg/LcStore | https://discord.gg/kYKWhyM2D4**

---

## 📜 ترخيص

هذا المورد مخصص للاستخدام في خادم FiveM فقط. لا يجوز بيع أو إعادة توزيع هذا المورد دون إذن صريح.

---

# 🐐 Lc-Eid | AboMalak

A complete script to celebrate Eid al-Adha inside FiveM servers. Includes giving Eidiya, sacrificing animals, and utilizing a targeting system compatible with popular systems.

---

## ✨ Features

- 🎁 Distribute Eidiya to players via NPCs.
- 🔪 Sacrifice animals using specific weapons.
- 🔄 Supports 4 targeting systems:
  - [interact](https://github.com/JacobWilliams/interact)
  - [Lc-target](https://github.com/Lc-Scripts/Lc-target)
  - [qb-target](https://github.com/qbcore-framework/qb-target)
  - [ox_target](https://github.com/overextended/ox_target)
- 🐐 Spawn goats/sheep in configurable locations.
- 🌍 Set multiple sacrifice zones and NPCs.
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
    ['image'] = 'meat_goat.png',
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

---

## ✅ Notes

- Ensure the images (`meat_goat.png`, `pancakes.png`) exist in your inventory's image folder.
- Players must have specific weapons to sacrifice the animal (e.g., `weapon_knife`, `weapon_machete`).
- You can select your preferred Target system via `Config.TargetSystem` in `config.lua`.

---

## 📌 Developer

- Developed by: **AboMalak | LcStore**
- Discord Support: **https://discord.gg/LcStore | https://discord.gg/kYKWhyM2D4**

---

## 📄 License

This resource is for use in FiveM servers only. Reselling or redistribution is not permitted without explicit permission.
