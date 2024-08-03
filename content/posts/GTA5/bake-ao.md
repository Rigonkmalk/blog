---
title: "GTA5 / Blender - Bake Fake AO"
date: 2024-04-03T16:30:00+01:00
draft: false
author: "Paul ( Rigonkmalk ) Azema"
---

# Bake Fake AO

<u>Description</u> :

C'est une méthode permettant la création d'ombre non dynamique pour éviter de surcharger les composants GPU de votre machine sur GTA5 lors de vos créations d'intérieur.

## Méthodologie

Vous devez créer un mesh ( pour cette explication, on va rester sur le sol ) de votre zone où vous souhaitez rendre vos ombres.

Ce mesh va avoir une configuration comme-ci dans votre material Blender que vous allez créer :

![materials.png](/blog/img/ao/materials.png)

Vous allez faire en sorte d'avoir une lumière extrêmement puissante qui va balancer du blanc avec la configuration suivante :

![Cast Configuration](/blog/img/ao/cast.png)

Dans votre scène, vous allez configurer votre render engine comme ceci :

![render engine](/blog/img/ao/render1.png)

![light path](/blog/img/ao/render2.png)

![Bake](/blog/img/ao/render3.png)

Vous pouvez créer une texture en 2K ou 4K pour le rendu, la taille permet d'avoir du détail.

Pour la suite, il va vous falloir inverser les couleurs depuis un logiciel d'édition photo ( NDLR : Photoshop par exemple ).

Exemple après inversion :

![Inversion example](/blog/img/ao/invert.png)

Sachant que la zone blanche sont les ombres.

Pour le shader GTA 5 : decal_dirt.sps avec un vertex color en noir.

