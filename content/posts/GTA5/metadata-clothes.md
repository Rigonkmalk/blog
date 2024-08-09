---
title: "GTA5 - Metadata Clothes"
date: 2024-08-08T10:05:00+01:00
draft: false
author: "Paul ( Rigonkmalk ) Azema"
---

# Description

L'idée de cet article est un processus qui permet de comprendre où et comment fonctionne les vêtements (on part du concept des chaussures à talon qui ont la nécessité d'avoir quelques fichiers en plus).

## Contenu du dossier de mods

```shell
.:
total 0
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 .
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 ..
-rwxrwxrwx 1 beta beta  206 Aug  9 11:04 fxmanifest.lua
-rwxrwxrwx 1 beta beta  429 Aug  9 11:04 mp_f_freemode_01_mp_f_soz_custom2.meta
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 stream

./stream:
total 4
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 .
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 ..
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 creaturemetadata
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 mp_f_freemode_01_mp_f_soz_custom2
-rwxrwxrwx 1 beta beta  787 Aug  9 11:04 mp_f_freemode_01_mp_f_soz_custom2.ymt

./stream/creaturemetadata:
total 0
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 .
drwxrwxrwx 1 beta beta 4096 Aug  9 11:04 ..
-rwxrwxrwx 1 beta beta  346 Aug  9 11:04 mp_creaturemetadata_soz_custom.ymt

./stream/mp_f_freemode_01_mp_f_soz_custom2: # fichiers stream
total 412
drwxrwxrwx 1 beta beta  4096 Aug  9 11:04  .
drwxrwxrwx 1 beta beta  4096 Aug  9 11:04  ..
-rwxrwxrwx 1 beta beta 49624 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_000_u.ydd'
-rwxrwxrwx 1 beta beta 39256 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_a_uni.ytd'
-rwxrwxrwx 1 beta beta 39410 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_b_uni.ytd'
-rwxrwxrwx 1 beta beta 39796 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_c_uni.ytd'
-rwxrwxrwx 1 beta beta 40518 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_d_uni.ytd'
-rwxrwxrwx 1 beta beta 34651 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_e_uni.ytd'
-rwxrwxrwx 1 beta beta 38474 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_f_uni.ytd'
-rwxrwxrwx 1 beta beta 39432 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_g_uni.ytd'
-rwxrwxrwx 1 beta beta 39501 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_h_uni.ytd'
-rwxrwxrwx 1 beta beta 41219 Aug  9 10:56 'mp_f_freemode_01_mp_f_soz_custom2^feet_diff_000_i_uni.ytd'
```

### fxmanifest.lua

```lua
fx_version 'cerulean'
game { 'gta5' }

files {
  'mp_f_freemode_01_mp_f_soz_custom2.meta'
}

data_file 'SHOP_PED_APPAREL_META_FILE' 'mp_f_freemode_01_mp_f_soz_custom2.meta'
```

### mp_f_freemode_01_mp_f_soz_custom2.meta

Ce fichier permet de définir le DLC et le contenu apporté au serveur fiveM pour appeler tout le contenu des vêtements.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<ShopPedApparel>
	<pedName>mp_f_freemode_01</pedName> <!-- On défini le sexe du DLC -->
    <!-- mp_f : female -->
    <!-- mp_m : male -->
	<dlcName>mp_f_soz_custom2</dlcName> <!-- Nom du DLC -->
	<fullDlcName>mp_f_freemode_01_mp_f_soz_custom2</fullDlcName> <!-- Nom du DLC au complet et doit avoir le nom complet du .ymt dans stream/mp_f_freemode_01_mp_f_soz_custom2.ymt -->
	<eCharacter>SCR_CHAR_MULTIPLAYER_F</eCharacter> <!-- On défini le sexe du DLC -->
    <!-- SCR_CHAR_MULTIPLAYER_F : female -->
    <!-- SCR_CHAR_MULTIPLAYER_M : male -->
	<creatureMetaData>MP_CreatureMetadata_soz_custom</creatureMetaData> <!-- Nom du creatureMetaData au complet et doit avoir le nom complet du .ymt dans stream/creaturemetadata/mp_creaturemetadata_soz_custom.ymt -->
	<pedOutfits>
	</pedOutfits>
	<pedComponents>
	</pedComponents>
	<pedProps>
	</pedProps>
</ShopPedApparel>
```

### stream/mp_f_freemode_01_mp_f_soz_custom2.ymt

Ce fichier permet de définir les variantes et les propriétés des objets qui seront streamé.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<CPedVariationInfo name="mp_f_soz_custom2">
 <bHasTexVariations value="true" />
 <bHasDrawblVariations value="false" />
 <bHasLowLODs value="false" />
 <bIsSuperLOD value="false" />
 <availComp>255 255 255 255 255 255 0 255 255 255 255 255</availComp>
 <!-- 255 : valeur nulle pour définir que les objets stream ne correspondent pas au fichier
 0 : L'objet appelé (ici feet) -->
 <aComponentData3 itemType="CPVComponentData">
  <Item>
   <numAvailTex value="9" /> <!-- Nombre de texture défini dans l'objet, le maximum étant 26 a-z -->
   <aDrawblData3 itemType="CPVDrawblData">
    <Item>
     <propMask value="1" />
     <numAlternatives value="0" />
     <aTexData itemType="CPVTextureData"> <!-- Cette liste correspond aux nombre de textures disponible pour l'objet -->
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
      <Item>
       <texId value="0" />
       <distribution value="255" />
      </Item>
     </aTexData>
     <clothData>
      <ownsCloth value="false" />
     </clothData>
    </Item>
   </aDrawblData3>
  </Item>
 </aComponentData3>
 <aSelectionSets itemType="CPedSelectionSet" />
 <compInfos itemType="CComponentInfo"> <!-- Les propriétés de l'objet -->
  <Item>
   <pedXml_audioID>shoe_high_heels</pedXml_audioID> <!-- Son de l'objet -->
   <pedXml_audioID2 />
   <pedXml_expressionMods>0 0 0 0 1.2</pedXml_expressionMods> <!-- Expression de l'objet 
   ici 1.2 correspond à la hauteur du talon -->
   <flags value="0" />
   <inclusions>0</inclusions>
   <exclusions>0</exclusions>
   <pedXml_vfxComps>PV_COMP_HEAD</pedXml_vfxComps>
   <pedXml_flags value="0" />
   <pedXml_compIdx value="6" />
   <pedXml_drawblIdx value="0" />
  </Item>
 </compInfos>
 <propInfo>
  <numAvailProps value="0" />
  <aPropMetaData itemType="CPedPropMetaData" />
  <aAnchors itemType="CAnchorProps" />
 </propInfo>
 <dlcName>hash_52893E2A</dlcName> <!-- nom du dlc -->
</CPedVariationInfo>
```

### stream/creaturemetadata/mp_creaturemetadata_soz_custom.ymt

Ce fichier est OBLIGATOIRE si vous définissez un objet avec des propriétés (comme pour les talons).

```xml
<?xml version="1.0" encoding="UTF-8"?>
<CCreatureMetaData>
 <pedCompExpressions>
  <Item>
   <pedCompID value="0x6" />
   <pedCompVarIndex value="0x0" />
   <pedCompExpressionIndex value="0x4" />
   <tracks content="char_array">
    33
   </tracks>
   <ids content="short_array">
    28462
   </ids>
   <types content="char_array">
    2
   </types>
   <components content="char_array">
    1
   </components>
  </Item>
 </pedCompExpressions>
 <pedPropExpressions />
</CCreatureMetaData>
```