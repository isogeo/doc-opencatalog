---
description: Présentation générale des prérequis pour l'installation de l'OpenCatalog
---

# Prérequis {#requirements}

## Navigateurs supportés

Pour accéder à un OpenCatalog, les navigateurs supportés sont :

* Mozilla Firefox 82 et + ;
* Google Chrome 86 et + ;
* Edge 86 et + ;

![Navigateurs supportés](/assets/requirements/supportedBrowsers.PNG)

> Astuce : si vous ou vos utilisateurs ne possèdent pas les droits suffisants pour mettre à jour le navigateur, vous pouvez utiliser une version portable (sans installation mais aux performances réduites) de [Mozilla Firefox](http://portableapps.com/apps/internet/firefox_portable/localization).

## Connexion Internet

Un débit descendant minimum de **500 Kb/s** est requis pour accéder à OpenCatalog.

## Services géographiques pris en charge

L'OpenCatalog permet l'exploitation des couches de services cartographiques pour visualiser et extraire les données. Les services suivants peuvent être exploités :

* les services de type Feature issues d'un service OGC, WFS ou Esri, Esri Feature Service autorisant l'extraction des données au format json/geojson ou GML3,
* les services de type Map issues d'un service OGC, WMS, ou Esri, Esri Map Service,
* les services tuilées issues d'un service OGC, WMTS ou d'un service Esri, Esri Tile Service.

Les services en question doivent être publics et ouverts pour être accessibles depuis l'OpenCatalog en mode de base. Le [mode no-proxy](/usage/generate.md#no-proxy) permet cependant d'accès à la visualisation et l'extraction des services internes non publics (locaux) non soumis à une authentification. 

Les groupes de couche ne sont pas actuellement pris en compte, seules les couches sont exploitables. 
