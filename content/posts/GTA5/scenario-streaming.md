---
title: "GTA5 - Scenario"
date: 2024-08-03T20:43:13+01:00
draft: false
author: "Paul ( Rigonkmalk ) Azema"
---

# FR

Vous aurez besoin de :

- sp_manifest.ymt
- government_facility.ymt

Dans le fichier sp_manifest.ymt, vous avez tel contenu :

```xml
  <Item type="CScenarioPointRegionDef">
   <Name>platform:/levels/gta5/scenario/government_facility</Name>
   <AABB>
    <min x="2386.979" y="-1002.365" z="-22.66828" />
    <max x="3466.869" y="909.7826" z="108.1135" />
   </AABB>
  </Item>
```

Si tu veux en streamer un, il faut changer vers quelque chose comme ça ( et augmenter la valeur AABB si vous augmenter la taille du scénario ):

```xml
  <Item type="CScenarioPointRegionDef">
   <Name>compcache:/government_facility</Name>
   <AABB>
    <min x="2386.979" y="-1002.365" z="-22.66828" />
    <max x="3466.869" y="909.7826" z="108.1135" />
   </AABB>
  </Item>
```

Donc en gros tu as 1 sp_manifest dans lequel tu modifie les scénarios que tu veux stream.
Tu dois mettre tes fichiers dans le même dossier et dans le fxmanifest.lua il te faut mettre :

```lua
data_file 'SCENARIO_POINTS_OVERRIDE_FILE' 'stream/companies/gouv/sp_manifest.ymt'

files {
...
    'stream/companies/gouv/sp_manifest.ymt',
...
}
```

---

# EN

You need :

- sp_manifest.ymt
- government_facility.ymt

In `sp_manifest.ymt` configuration you will have this :

```xml
  <Item type="CScenarioPointRegionDef">
   <Name>platform:/levels/gta5/scenario/government_facility</Name>
   <AABB>
    <min x="2386.979" y="-1002.365" z="-22.66828" />
    <max x="3466.869" y="909.7826" z="108.1135" />
   </AABB>
  </Item>
```

If you want to stream a new one, you will need to change the name and the min max ( if you increase the AABB size ) :

```xml
  <Item type="CScenarioPointRegionDef">
   <Name>compcache:/government_facility</Name>
   <AABB>
    <min x="2386.979" y="-1002.365" z="-22.66828" />
    <max x="3466.869" y="909.7826" z="108.1135" />
   </AABB>
  </Item>
```
You 
And in `fx_manifest.lua` you need to put this :

```lua
data_file 'SCENARIO_POINTS_OVERRIDE_FILE' 'stream/companies/gouv/sp_manifest.ymt'

files {
...
    'stream/companies/gouv/sp_manifest.ymt',
...
}
```