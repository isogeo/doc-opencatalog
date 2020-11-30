# Notes des version

<!-- timeline -->

## 3.1.0 {#v310}

Publiée en décembre 2020 :

### OpenCatalog

* refonte complète de l'OpenCatalog en utilisant la bibliothèque JavaScript React
* passage à l'API cartographique [OpenLayers](https://openlayers.org/)
* amélioration de la visualisation de couches issues de géoservices
* amélioration de l'extraction des Feature Services
* meilleure prise en compte des services ESRI (Esri Feature Service et Esri Map Service)
* ajout d'un nouveau paramètre d'URL `dataset-only` permettant de masquer les geoservices dans les résultats de l'OpenCatalog

<!-- /timeline -->

<!-- timeline -->

## 2.3.2 {#v232}

Publiée en décembre 2017 :

### OpenCatalog

* ajout d'un nouveau paramètre' d&apos;URL `no-proxy` à OpenCatalog permettant de passer outre les proxies intégrés afin de consommer les services internes

<!-- /timeline -->

<!-- timeline -->

## 2.3.0 {#v230}

Publiée fin juillet 2017.

### Modifications

* refonte complète de l&apos;ergonomie et de l&apos;interface :
  * les sections d&apos;une fiche de métadonnées sont piables/dépliables
  * ajout d&apos;un bouton pour copier/coller les URLs des capacités des services
  * ajout des vignettes basées sur l&apos;emprise
  * navigation réciproque entre métadonnée d&apos;un jeu de données et métadonnées des services associés

* bascule du widget de recherche sur celui d&apos;APP avec notamment l&apos;ajout du tri des résultats et de l&apos;auto-complétion
* mise en cohérence de la construction des URLs (structure et paramètres)
* refonte de la visualisation des couches de service
* ajout d&apos;un formulaire de téléchargement des données vectorielles généré automatiquement à partir des WFS
* refactoring complet du code source

<!-- /timeline -->

<!-- timeline -->

## 2.2. {#v22}

Publiée fin mars 2017.

Consulter :

* le [mail envoyé aux utilisateurs](http://us4.campaign-archive1.com/?u=256352d96aabf0dec0ee32d84&id=b57277a32c)

### Modifications

* refonte de la prévisualisation intégrée des services géographiques :

  * mise à jour des dépendances (Leaflet et plugins associés)
  * définition plus précise du cas générique selon les formats et versions
  * meilleure gestion des cas particuliers (SRS incompatibles, etc.)

<!-- /timeline -->

<!-- timeline -->

## 2. {#v2}

Publiée en septembre 2016.

Consulter :

* le [mail envoyé aux utilisateurs](http://us4.campaign-archive1.com/?u=256352d96aabf0dec0ee32d84&id=1a0a2c1231)

### Modifications

* les liens de visualisation des services géographiques rencensés et associés avec la nouvelle méthode sont automatiquement générés dans le bouton "Visualiser"
* si le service WFS associé le permet, un lien de téléchargement de la donnée brute est automatiquement généré dans le bouton "Télécharger".

<!-- /timeline -->

<!-- timeline -->

## 2. {#v2}

Publiée en juillet 2016.

Consulter :

* le [mail envoyé aux utilisateurs](http://eepurl.com/b7NoAD)
* le [mail envoyé aux administrateurs du Scan FME](http://eepurl.com/b8uYqb).

### Modifications

* les résultats d&apos;une recherche par désormais trier par "pertinence" puis par "date de création de la fiche de métadonnée (ordre décroissant)" : fonctionnement identique à APP
* dans une fiche de métadonnées, possibilité de :
  * trier la liste des champs attributaires (comportement identique à celui de APP)
  * revenir en haut de la page

<!-- /timeline -->

<!-- timeline -->

## 2. {#v2}

Publiée en avril 2016.

Consulter :

* le [mail envoyé aux utilisateurs](http://us4.campaign-archive2.com/?u=256352d96aabf0dec0ee32d84&id=4c66022137).

### Modifications

* conforme au WCAG 2.0 niveau AA
* Sécurisation du proxy Open Catalog

<!-- /timeline -->

<!-- timeline -->

## 2. {#v2}

Publiée le 16 octobre 2015.

Consulter :

* le [mail envoyé aux utilisateurs](https://us4.campaign-archive2.com/?u=256352d96aabf0dec0ee32d84&id=12e0fad409).

### Modifications

* Changement dynamique du fond de plan
* Ajout de pages d&apos;erreur pour les ressources introuvables et pour les connexions lentes

<!-- /timeline -->

<!-- timeline -->

## 2. {#v2}

Publiée le 10 juillet 2015.

Consulter :

* le [mail envoyé aux utilisateurs](http://eepurl.com/brcEPr).

### Modifications

* choix du fond de plan parmi :
  * Bing Maps Road (par défaut) vue classique
  * Bing Maps Aerial vue satellite
  * OpenStreetMap.BlackAndWhite vue noir et blanc
  * OpenMapSurfer.road
  * vide (utile pour les services de carte sans transparence)
* mise en place d&apos;une page "ressource introuvable"

<!-- /timeline -->

<!-- timeline -->

## 2.0 {#v20}

Publiée le 27 mars 2015.

Consulter :

* le [mail envoyé aux utilisateurs](http://eepurl.com/bhQtIn).

### Modifications

* mise en production de la version 2 : voir [le mailing associé](http://eepurl.com/bfpoQb).
* utilisation des filtres présents dans les fiches de métadonnées
* affichage des services cartographiques issus de Business Geographic


<!-- /timeline -->

<!-- timeline -->

## 1. {#1}

Publiée fin décembre 2014.

Consulter :

* le [mail envoyé aux utilisateurs](http://us4.campaign-archive1.com/?u=256352d96aabf0dec0ee32d84&id=45f2788b69)
* la [vidéo du webinaire](http://youtu.be/1BTwZqii0EY) présentant les principales nouveautés :

### Modifications

* Possible de visualiser les flux WMTS.
* Page de résultats : les traits entre les fiches de métadonnées s&apos;affichent
* Les couleurs des boutons "Actions" sont bien gérées
* Les flux WFS s&apos;affichent sur la carte si au format JSONP
* Le bouton "Plein écran" s&apos;affiche dans la carte
* Les liens associés s&apos;affichent dans les actions

<!-- /timeline -->

<!-- timeline -->

## 1. {#v1}

Publiée fin septembre 2014.

Consulter :

* le [mail envoyé aux utilisateurs](http://us4.campaign-archive2.com/?u=256352d96aabf0dec0ee32d84&id=fabb845b06)
* la [vidéo du webinaire](http://youtu.be/l6vmlYwUHDM?list=PLouu1QiHcsHSDGdvysTn1KRhr3JQUDol4) présentant les principales nouveautés :

### Modifications

* il est désormais possible de gérer l&apos;affichage des ressources selon les usages,

> A l&apos;étude : édition par lot et planification

<!-- /timeline -->

<!-- timeline -->

## 1. {#v1}

Publiée en juillet 2014.

Consulter :

* le [mail envoyé aux utilisateurs](http://us4.campaign-archive1.com/?u=256352d96aabf0dec0ee32d84&id=6dc56a2972)

### Modifications

* mise en valeur des ressources associées via des boutons de visualisation, téléchargement et autres,
* possiblité de personnaliser la couleur du thème,
* le nom du bandeau est celui du partage,

<!-- /timeline -->
