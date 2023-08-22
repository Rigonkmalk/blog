---
title: "CSV"
date: 2023-08-22T14:40:00+02:00
draft: false
author: "Paul ( Rigonkmalk ) Azema"
---

On va commencer le blog sur un article qui tout particulièrement me chagrine.

# CSV - On t'aime, mais pas tellement

Le CSV, si vous avez déjà bossé dessus, vous saurez ce que je veux dire par le "je t'aime".

Le CSV c'est un peu comme une histoire entre deux personnes qui peuvent se comprendre, mais va falloir décoder quelques trucs.

## Qu'est-ce qui ne va pas avec le CSV ?

Rien du tout ! Tout va bien avec le CSV… 'fin… presque.

## Les séparateurs

Quand généralement on parle CSV, on entend souvent parler de "CSV, c'est une virgule qui sépare les champs" *insérer doigt en l'air, yeux fermé, sourire satisfait*.

Alors oui, j'entends très bien, mais ayant discuté avec d'autres personnes et collègues dans mon entourage,
c'est aussi un autre son de cloche.

`On peut aussi utiliser ; , mais aussi \<TAB>, mais aussi |`

Je suis d'accord aussi *racle la gorge*, mais… le nom CSV porte bien son nom ?

```
   This RFC documents the format used for Comma-Separated Values (CSV)
   files and registers the associated MIME type "text/csv".
```
cf. [rfc7111](https://datatracker.ietf.org/doc/html/rfc7111)

Donc, on est bien d'accord, "Comma = ," ? Et bien, il faut noter que cette RFC7111, n'est qu'un Memo
et non un standard, ainsi, nos amis les informaticiens, généralement, quand tu leur laisses une marge, bah ils la prennent.

Et ils y foutent ce qu'ils veulent pour faire office de séparateur, et ça va généralement poser des soucis entre 2 softs.

Tu vas avoir les softs qui vont suivre le Memo à la lettre, et tu as les autres qui vont chercher sur un moteur de recherche

`How can I separate in CSV in other way than comma ?`

Et là, patatra ! Tout le monde y met du sien parce que ça fonctionne malgré s le fait que tu ne mettes pas une virgule !

## Anecdote personnelle

Il n'y a pas longtemps, j'ai dû mettre en place un annuaire de numéro et de contact provenant d'un "programme" fait en Windev,
et notre cher ami qui a pondu le "programme" (NDLR Je hais Windev et leur côté misogyne assumé) me sortais un fichier .csv
avec pour séparateur des ";".

Moi, bêtement, je tente de l'importer sur ma solution, qui, elle, a été faite en lisant le Memo, et bien… bah ça marche po.

Après, petites recherche et analyse du fichier, j'ai remarqué le séparateur, un simple cherche et remplacer pour passer ; => ,.

Alors certes, c'est rapide, mais c'est chiant quand tu veux monter quelque chose assez rapidement et que tu as un partenaire commercial,
qui vient te faire chier pour un truc aussi chiant "ça ne marche pas, résout moi les soucis et vite, c'est urgent", pas pour moi mon coco.
