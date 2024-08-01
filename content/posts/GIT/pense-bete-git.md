---
title: "Pense-Bête Git"
date: 2024-08-01T18:35:27+01:00
draft: false
author: "Paul ( Rigonkmalk ) Azema"
---

# Pense-Bête

Je me retrouve parfois perdu dans mes commandes Git et ce que je pourrais en faire plus tard. Je me retrouve TRÈS souvent à utiliser un bon vieux \<C-r\> dans mon terminal pour tenter de retrouver ce que je cherche !

L'article aura pour objectif de s'améliorer afin de suivre les nouvelles commandes pouvant m'être utiles.

> Comme quoi, la frustration peux aider :)

```shell
git fetch origin main
```

Permet d'aller chercher les derniers commit dans la branch `main` ( main étant bien sûr changeable ).

```shell
git pull
```

Permet de récupérer tout les dernières branch ET commit de la branche active.

```shell
git rebase refs/heads/main
```

Permet de récupérer les derniers commit de la branch `main` dans la branche active.