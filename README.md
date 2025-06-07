# 🐐 Lc-Eid | سكربت عيد الأضحى لـ FiveM

سكربت متكامل لإحياء فعاليات عيد الأضحى داخل سيرفرات FiveM. يتضمن توزيع العيدية، ذبح الأضحية، واستعمال نظام التارقت المتوافق مع أشهر الأنظمة.

---

## ✨ المميزات

- 🎁 توزيع عيديات للاعبين من خلال NPC.
- 🔪 ذبح الأضاحي باستخدام أسلحة محددة.
- 🔄 دعم ثلاث أنظمة Target:
  - `interact`
  - `Lc-target`
  - `ox_target`
- 👤 تخصيص كامل عبر ملف `config.lua`.
- 🐐 ظهور خروف/ماعز في مواقع محددة.
- 🌍 إمكانية تحديد مناطق و NPC مختلفة.

---

## ⚙️ التركيب

-- qb-core/shared/item.lua
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

-- qb-core/server/main.lua
```
QBCore.Functions.CreateUseableItem('meat_goat', function(source, item)
    local Player = QBCore.Functions.GetPlayer(source)
    if Player.Functions.AddItem(item.name, 1) then
        TriggerClientEvent('inventory:client:ItemBox', source, QBCore.Shared.Items[item.name], 'add')
    end
end)
```
