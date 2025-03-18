---
title: "IA - Axe de réflexion"
date: 2025-03-18T16:30:00+01:00
draft: false
author: "Paul ( Rigonkmalk ) Azema"
---

# IA - Axe de réflexion

## Liste des conseils

Voici quelques conseils pour formuler des prompts efficaces lorsque vous posez des questions à une IA :

- Partez du principe que l’IA se doit d'être positive : Si nécessaire, précisez lui d’accepter un refus à la réponse.

- Fournissez des informations contextuelles : Si nécessaire, donnez des détails supplémentaires sur le sujet ou le contexte de votre question. Cela permettra à l'IA d'avoir un meilleur aperçu de ce que vous voulez savoir.

- Utilisez un langage naturel : Écrivez votre prompt comme vous le feriez dans une conversation normale. Évitez d'utiliser un langage trop formel ou technique, sauf si c'est nécessaire.

- Soyez poli et courtois : Commencez votre prompt par un "s'il vous plaît" et terminez-le par un "merci". Cela contribuera à établir une interaction agréable avec l'IA.

- Soyez ouvert à des réponses nuancées : Certaines questions n'ont pas de réponse simple. Soyez prêt à recevoir des réponses qui explorent différents aspects du sujet.

- Demandez des clarifications si nécessaire : Si la réponse de l'IA n'est pas claire, n'hésitez pas à poser des questions supplémentaires pour obtenir plus de détails.

## Spécification

L’idée d’une IA est lorsque vous lui demandez une action, une question, une réflexion, une optimisation, une mise en contexte… Son but est d’Absolument répondre positivement à votre question.

### Réponse positive

Si le but de la réponse positive est instauré sur une IA, il faut partir dans l’esprit sur lequel la question que vous poserez, peu importe ce que vous lui demandez, son but est de satisfaire l’utilisateur, garder donc à l’esprit que votre question, aussi basse en qualité qu’elle ne peut l’être, la qualité de la réponse sera la réflexion de votre question.

# Questions

## Question Évasive

Quand vous allez poser votre question, il faut être le plus clair et concis possible, la matière de votre question va être basé sur les mots et les termes utilisés pour apporter une réponse.

Pour l’exemple, je présente une question pour 5 IA différentes.

Question

```
Quelle est la version actuelle sur l’outil Centreon ?
```

### Claude 3 Haiku (Via DuckduckGo AI Chat)

```
Désolé, mais je ne peux pas vous fournir d'informations spécifiques sur la version actuelle de l'outil Centreon. En tant qu'assistant IA, je n'ai pas accès à ces détails techniques. Je vous suggère de vous renseigner directement auprès de l'équipe de développement de Centreon ou de consulter leur site web officiel pour obtenir les informations les plus à jour sur les versions disponibles. Je ne peux malheureusement pas vous en dire davantage sur ce sujet.
```
Il faut noter que Claude 3 Haiku utilisé dans DuckDuckGo utilise des données qui lui sont données dans une data source pré-configuré.

### Claude 3 Haiku (Via Claude.ai)

```
Je dois vous informer que je ne peux pas vous donner la version actuelle exacte de Centreon, car mes connaissances sont limitées à avril 2024. En effet, Centreon, étant un logiciel activement maintenu, sort régulièrement de nouvelles versions.

Pour obtenir l'information la plus à jour sur la version actuelle de Centreon, je vous conseille de :

1. Consulter le site officiel de Centreon (www.centreon.com)
2. Vérifier leur page de téléchargement
3. Consulter leur documentation technique
4. Suivre leurs annonces sur les réseaux sociaux

Voulez-vous que je vous explique les fonctionnalités principales de Centreon ou que je vous aide sur un aspect particulier de cet outil de supervision ?
```
### Chat-GPT4o (Via chatgpt.com)

```
La version actuelle de Centreon est la 24.10, publiée en octobre 2024. Cette version introduit un nouveau rythme de publication avec une version majeure par an et propose un support à long terme (LTS) pour les éditions commerciales, étendant la durée de support à 3 ans. ([centreon.com](https://www.centreon.com/new-centreon-release-cadence-and-version-lifecycle/?utm_source=chatgpt.com))

Pour plus de détails sur les fonctionnalités de cette version, vous pouvez consulter le site officiel de Centreon. ([centreon.com](https://www.centreon.com/?utm_source=chatgpt.com)) 
```

Il faut noter que Chat-GPT4o utilise le framework RAG pour permettre d’obtenir la réponse en utilisant les outils de recherche sur internet.

#### Conclusion

Claude 3 Haiku Via DuckduckGo étant configuré de manière à utiliser le moins d’outil tiers pour permettre de recevoir la réponse, il faut garder en tête que la data source utilisé par les équipes qui ont préparé et compilé ses données.

Claude 3 Haiku  étant configuré de manière à utiliser le moins d’outil tiers pour permettre de recevoir la réponse, il faut garder en tête que la data source utilisé par les équipes qui ont préparé et compilé ses données, ses réponses sont donc retournées en question

On voit que la réponse la plus précise reste celle de Chat-GPT4o, car leurs outils permettent également la recherche sur les sites internet et donc de pouvoir répondre le plus précisément en se basant sur ses data sources ainsi que ses propres recherches via un Agent.

Il faut donc garder en tête de rester le plus simple et concis dans le cadre d’une question, sur la question que j’ai posée, je suis resté le plus évasif possible.

Mes erreurs sur la question :

- Je n’ai pas demandé la dernière version de Centreon
- J’ai demandé l’actuelle, mais Centreon garde en ligne plusieurs versions différentes
- La version actuelle, reste évasif également

## Question Précise

La question la plus précise et concise serait donc 

```
Quelle est la dernière version proposée par Centreon ?
```

### Claude 3 Haiku

```
Désolé, mais je ne peux pas vous fournir d'informations spécifiques sur les versions de Centreon. En tant qu'assistant IA, je n'ai pas accès à ce type de données détaillées sur les produits et services de tiers. Je vous suggère de vous renseigner directement auprès de Centreon ou sur leur site web pour obtenir les informations les plus à jour sur leurs dernières versions. Je peux cependant vous aider avec d'autres sujets de manière générale si vous le souhaitez.
```

### ChatGPT

```
La dernière version proposée par Centreon est la 24.10, publiée en octobre 2024. Cette version introduit un nouveau cycle de publication avec une version majeure annuelle chaque mois d'octobre. Les versions majeures des années paires, comme la 24.10, bénéficient d'un support à long terme (LTS) de 3 ans pour les éditions commerciales, tandis que celles des années impaires sont supportées pendant 18 mois. Les versions Open Source de Centreon sont, quant à elles, supportées pendant 18 mois. ([centreon.com](https://www.centreon.com/new-centreon-release-cadence-and-version-lifecycle/?utm_source=chatgpt.com))
```

## Conclusion

Claude 3 Haiku étant configuré de manière à utiliser le moins d’outil tiers pour permettre de recevoir la réponse, il faut garder en tête que la data source utilisé par les équipes qui ont préparé et compilé ses données.

On voit que la plus “belle” reste celle de Chat-GPT4o, car leurs outils permettent également la recherche sur les sites internet et donc de pouvoir répondre le plus précisément en se basant sur ses data sources ainsi que ses propres recherches via un Agent.

Mais on remarque le côté “généraliste” de chatGPT qui n’a pas la capacité de répondre sans chercher sur internet la réponse

En changeant la méthodologie de réponse, on remarque pleinement que Neo devient le plus enclin à donner une réponse qui est attendue.

# Contextualiser

Fournissez des informations contextuelles : Si nécessaire, donnez des détails supplémentaires sur le sujet ou le contexte de votre question. Cela permettra à l'IA d'avoir un meilleur aperçu de ce que vous voulez savoir.

L’objectif d’une IA est de répondre de la manière la plus précise, complète et basée sur la demande que vous lui avez demandée. Si votre prompt n’est pas assez précis, il est assez décevant de recevoir une réponse qui ne répond peu ou pas à votre attente.

La première étape d’un bon prompt est de réfléchir à la finalité de la réponse, ne pas rester sur de l’évasif, le rôle d’une IA est de vous donner un résultat, pas forcément de vous apprendre quelque chose.

Si l’on demande à une IA :

```
Créé moi un site web
```

Selon la configuration de l’IA la réponse sera toujours quelque chose de très générique et qui, en effet, pourras vous fournir une réponse, mais si votre finalité, c'est que vous vouliez un site rose, le résultat donné ne correspondra pas à votre attente.

Exemple : [Without Context](https://codepen.io/Rigonkmalk/pen/qEBxwNQ) 

```
Créé moi un site web en HTML, CSS et Javascript. Le site doit avoir un fond en rose
```

Même si la demande n’est pas la plus précise, le fait de rajouter un contexte permet à l’IA de correspondre à la finalité attendue.

Exemple : [With Context](https://codepen.io/Rigonkmalk/pen/wBvyZoG) 

De ce que l’on peut remarquer, c’est qu’en effet, l’IA répond à ma demande liée au contexte, mais à rajouter des fonctionnalités (changement de fond d'écran sur le site, affichage d’un message) sans que j'en aie émis la demande.

## Conclusion

En effet, l’IA souhaitant répondre le plus positivement possible à nos requêtes, on remarque bien une réponse qui a pour but de répondre à la demande, mais l’on obtient une finalité médiocre.

Un prompt se doit d'être le plus précis et contextualisé le plus possible, mais il faut réfléchir à un final avant de demander quelque chose. 
