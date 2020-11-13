# Générer un OpenCatalog
## Paramétrer la couleur
## Intégrer l'OpenCatalog dans un site (iframe)
OpenCatalog est développé via l’API Isogeo. Il est designé pour être facilement intégrable dans vos sites web existants (intranet, extranet, portail carto, portail OpenData, IDG, etc.) via une [balise HTML iFrame](https://www.w3schools.com/tags/tag_iframe.asp).

Plusieurs modes sont implementés dans l'OpenCatalog pour faciliter l'affichage dans une telle balise.

### Retirer la barre de titre
Il existe un mode permettant de retirer la barre de titre.

#### Utilisation du mode no-header
Pour utiliser ce mode, il suffit d'ajouter ``?no-header`` en paramètre à l'URL.

Par exemple, pour intégrer l'OpenCatalog de démonstration :
```
<iframe src="https://open.isogeo.com/s/344d51c3edfb435daf9d98d948fa207e/Sbd1w7PgqE8n7LDq3azRqNhiMHZf0?no-header" width=100% height="800"></iframe>
```

### Intégrer une page unique
Si vous ne souhaitez intégrer qu'une seule fiche par exemple dans une fenêtre de type pop-up, utiliser le mode ``?lock``.

Les différences suivantes sont à noter par raport à la version sans mode renseigné :
* La barre de titre est retiré
* La navigation d'une page à une autre est désactivée : Si la page est une fiche de métadonnée, il est impossible de retourner vers la liste des données du catalogue ou de se rendre à une autre donnée associée. Si la page unique est la page de recherche, il est impossible de se rendre sur une ressource.

#### Utilisation du mode lock
Pour utiliser ce mode, il suffit d'ajouter ``?lock`` à la fin de l'adresse.

Par exemple :
```
<iframe src="http://open.isogeo.com/s/344d51c3edfb435daf9d98d948fa207e/Sbd1w7PgqE8n7LDq3azRqNhiMHZf0/m/754209f115c040a48d43ffc262b16500?lock" height="400"></iframe></a>
```

### Désactiver le proxy
Pour récupérer les informations liées aux services cartographiques malgré les problèmes de Cross-Origin, l'OpenCatalog utilise un proxy. Cependant ce proxy empêche les requête aux services "locaux" (tout service uniquement disponible localement : que ce soit directement en local ou sur un serveur interne).  Pour avoir accès à ces services depuis le site, il faut désactiver le proxy.

#### Utilisation du mode no-proxy
Pour utiliser ce mode, il suffit d'ajouter ```?no-proxy``` à la suite du lien. Par exemple, pour intégrer le catalogue de démonstration :
```
<iframe src="https://open.isogeo.com/s/344d51c3edfb435daf9d98d948fa207e/Sbd1w7PgqE8n7LDq3azRqNhiMHZf0?no-proxy" width=100% height="400"></iframe>
```
#### Autoriser les requêtes Cross Origin
Désactiver le porxy peut causer des problèmes de Cross Origin. C'est pourquoi  il faut autoriser l'accès au server à l'OpenCatalog :
```
Access-Control-Allow-Origin: https://open.isogeo.com
```
Des informations à des serveurs spécifiques peuvent être trouvées [ici](https://fr.wikipedia.org/wiki/Cross-origin_resource_sharing).
