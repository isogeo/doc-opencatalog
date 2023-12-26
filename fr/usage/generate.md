---
description: Générer un OpenCatalog
---

# Générer un OpenCatalog

## Générer un catalogue de consultation avec OpenCatalog

Pour créer un OpenCatalog, il suffit de :

1. Dans le menu `Administration`  > `Inventaire` > `Partage`, cliquer sur `Nouveau` ;
2. Cliquer sur le bouton en forme d'engrenages ;
3. Sélectionner l’application `OpenCatalog` ;
4. Sélectionner le ou les catalogues à publier ;
5. Nommer le partage ;
6. `Enregistrer` ;

L'URL de consultation de l'OpenCatalog apparaît alors.

![Gérer les OpenCatalog](/assets/usage/generateOC.PNG)

> NB : En mode On-premises, l'URL de l'Opencatalog aura le même domaine que celui de la plateforme d'administration.

## Paramétrer la couleur

Il est possible d'intégrer l'OpenCatalog directement dans un site. Si vous souhaitez intégrer au mieux l'OpenCatalog dans la charte graphique de votre organisme, vous pouvez sélectionner la couleur principale du thème. Cette opération s'effectue dans le menu d'administration de la plateforme.

Pour changer la couleur principale du thème :

1. Dans le menu `Administration` > `Isogeo` > `Paramètres`, changer la couleur.

Pour revenir à la couleur par défaut, cliquer sur la croix dans le coin droit supérieur du widget de couleur.

![Modifier la couleur](/assets/usage/colorPicker.PNG)

## Intégrer l'OpenCatalog dans un site (iFrame)

L'OpenCatalog est développé via l’API Isogeo. Il a été créé pour être facilement intégrable dans vos sites web existants (intranet, extranet, portail carto, portail OpenData, IDG, etc.) via une [balise HTML iFrame](https://www.w3schools.com/tags/tag_iframe.asp).

Plusieurs modes sont implémentés dans l'OpenCatalog pour faciliter l'affichage dans un iFrame.

* Retirer la barre de titre
* Retirer les services, les ensembles de données et les ressources
* Désactiver le proxy

### Retirer la barre de titre

Il existe un mode permettant de retirer la barre de titre.

#### Mode no-header

Pour utiliser ce mode, il suffit d'ajouter ``?no-header`` en paramètre à l'URL.

Par exemple, pour intégrer l'OpenCatalog de démonstration :

```html
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?no-header" width=100% height="800"></iframe>
```

### Retirer les services et les ressources

Il existe cinq types de fiche dans l'API Isogeo :

* Donnée raster (et Ensemble de données)
* Donnée vecteur
* Ressource
* Service

Si vous souhaitez n'afficher les données rasters et vecteurs à la liste des résultats, vous pouvez utiliser le mode `dataset-only`.

#### Utilisation du mode dataset-only

Pour l'utiliser, il suffit d'ajouter ``?dataset-only`` à la fin de l'url de l'OpenCatalog.

Par exemple :

```html
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?dataset-only" width=100% height="800"></iframe></a>
```

### Désactiver le proxy

Pour récupérer les informations liées aux services cartographiques malgré les problèmes de [Cross-Origin](https://developer.mozilla.org/fr/docs/Web/HTTP/CORS) l'OpenCatalog utilise un proxy. Cependant, ce proxy empêche les requêtes aux services "locaux" (tout service uniquement disponible localement : que ce soit directement en local ou sur un serveur interne).  Pour avoir accès à ces services depuis le site, il faut désactiver le proxy.

#### Utilisation du mode no-proxy {#no-proxy}

Pour utiliser ce mode, il suffit d'ajouter `?no-proxy` à la fin de l'url.

Par exemple :

```html
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?no-proxy" width=100% height="800"></iframe>
```

#### Autoriser les requêtes Cross Origin

Désactiver le proxy peut causer des problèmes de [Cross-Origin](https://developer.mozilla.org/fr/docs/Web/HTTP/CORS). C'est pourquoi, il faut autoriser l'accès au serveur à l'OpenCatalog :

```bash
Access-Control-Allow-Origin: https://open.isogeo.com
```

> NB : Des informations spécifiques sur certains serveurs peuvent être trouvées [ici](https://fr.wikipedia.org/wiki/Cross-origin_resource_sharing).

## Intégrer une page unique (iFrame)

Si vous ne souhaitez intégrer qu'une seule fiche, par exemple, dans une fenêtre de type pop-up, utilisez le mode `?lock`.

Les différences suivantes sont à noter par rapport à la version par défaut :

* La barre de titre est retirée
* La navigation d'une page à une autre est désactivée : il est donc impossible de retourner vers la liste des données du catalogue, de cliquer sur un mot-clé ou encore de se rendre sur une autre fiche associée.  

### Mode lock {#lock}

Pour utiliser ce mode, il suffit d'ajouter ``?lock`` à la fin de l'adresse de l'url de la fiche.

Par exemple :

```html
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0/r/66d9aa8eb6d641d28b43632695b69833?lock" width=100% height="800"></iframe></a>
```
