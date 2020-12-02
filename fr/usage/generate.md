# Générer un OpenCatalog
## Générer un catalogue de consultation avec OpenCatalog
Pour créer un OpenCatalog, il suffit de :

1. Dans le menu `Administration`  > `Inventaire` > `Partage`, cliquer sur `Nouveau` ;
2. Cliquer sur le bouton en forme d&apos;engrenages ;
3. Sélectionner l’application `OpenCatalog` ;
4. Sélectionner le ou les catalogues à publier ;
5. Nommer le partage ;
6. `Enregistrer` ;

L&apos;URL de consultation de l&apos;openCatalog apparaît alors.

![Gérer les OpenCatalog](/assets/usage/generateOC.PNG)

## Paramétrer la couleur
Il est possible d'intégrer l'OpenCatalog directement dans un site. Si vous souhaitez intégrer au mieux les OpenCatalogs dans la charte graphique de votre organisme, vous pouvez sélectionner la couleur principale du thème.

Pour changer la couleur principale du thème :
1. Dans le menu `Administration` > `Isogeo` > `Paramètres`, changer la couleur.

Pour revenir à la couleur de base, cliquer sur la croix dans la roue de couleur.

![Modifier la couleur](/assets/usage/colorPicker.PNG)

## Intégrer l'OpenCatalog dans un site (iframe)
OpenCatalog est développé via l’API Isogeo. Il a été créé pour être facilement intégrable dans vos sites web existants (intranet, extranet, portail carto, portail OpenData, IDG, etc.) via une [balise HTML iFrame](https://www.w3schools.com/tags/tag_iframe.asp).

Plusieurs modes sont implementés dans l'OpenCatalog pour faciliter l'affichage dans une telle balise.

### Retirer la barre de titre
Il existe un mode permettant de retirer la barre de titre.

#### Utilisation du mode no-header
Pour utiliser ce mode, il suffit d'ajouter ``?no-header`` en paramètre à l'URL.

Par exemple, pour intégrer l'OpenCatalog de démonstration :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?no-header" width=100% height="800"></iframe>
```

### Intégrer une page unique
Si vous ne souhaitez intégrer qu'une seule fiche par exemple dans une fenêtre de type pop-up, utilisez le mode ``?lock``.

Les différences suivantes sont à noter par raport à la version sans mode renseigné :
* La barre de titre est retiré
* La navigation d'une page à une autre est désactivée : Si la page est une fiche de métadonnée, il est impossible de retourner vers la liste des données du catalogue ou de se rendre à une autre donnée associée. Si la page unique est la page de recherche, il est impossible de se rendre sur une ressource.

#### Utilisation du mode lock
Pour utiliser ce mode, il suffit d'ajouter ``?lock`` à la fin de l'adresse.

Par exemple :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?lock" height="400"></iframe></a>
```

### Retirer les services et ressources
Il existe quatre types de fiche sur la plateforme Isogeo :
* Donnée raster
* Donnée vecteur
* Ressource
* Service

Si vous souhaitez seulement afficher les données raster et vecteur sur votre page, vous pouvez utiliser le mode ``?dataset-only``.

#### Utilisation du mode dataset-only
Pour utiliser ce mode, il suffit d'ajouter ``?dataset-only`` à la fin de l'adresse.

Par exemple :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?dataset-only" height="400"></iframe></a>
```

### Désactiver le proxy
Pour récupérer les informations liées aux services cartographiques malgré les problèmes de Cross-Origin, l'OpenCatalog utilise un proxy. Cependant ce proxy empêche les requêtes aux services "locaux" (tout service uniquement disponible localement : que ce soit directement en local ou sur un serveur interne).  Pour avoir accès à ces services depuis le site, il faut désactiver le proxy.

#### Utilisation du mode no-proxy
Pour utiliser ce mode, il suffit d'ajouter ```?no-proxy``` à la suite du lien. Par exemple, pour intégrer le catalogue de démonstration :
```
<iframe src="https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0?no-proxy" width=100% height="400"></iframe>
```
#### Autoriser les requêtes Cross Origin
Désactiver le porxy peut causer des problèmes de Cross Origin. C'est pourquoi  il faut autoriser l'accès au server à l'OpenCatalog :
```
Access-Control-Allow-Origin: https://open.isogeo.com
```
Des informations à des serveurs spécifiques peuvent être trouvées [ici](https://fr.wikipedia.org/wiki/Cross-origin_resource_sharing).
