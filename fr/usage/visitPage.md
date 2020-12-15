---
description: Description de la page de consultation d'une fiche détaillée de l'OpenCatalog
---

# Consulter une fiche de métadonnée

Les fiches (de données, d’ensemble de données ou de services) sont présentées de manière à répondre aux besoins des spécialistes comme des non-spécialistes. Elles sont conformes INSPIRE et donnent accès aux fichiers XML ISO 19139.

Elles permettent également de mettre en valeur les ressources associées regroupées en 3 grandes actions :

* Visualiser
* Télécharger
* Accéder à des ressources externes.

![Consulter la fiche détaillée](/assets/usage/metadata.png)

## Champs

Les champs disponibles dépendent du type de la donnée. Pour chaque type de donnée, tous les champs remplissables depuis l'interface d'administration APP sont disponibles.

|  | Vecteur | Raster | Service | Ressource |
| ------ | :--------: |:------: | :-----------: | :------: |
| **Résumé** | - | - | - | - |
| Résumé | x | x | x | x |
| **Historique** | - | - | - | - |
| Date de création | x | x | x | x |
| Mise à jour | x | x | x | x |
| Début de validité | x | x |  |  |
| Fin de validité | x | x |  |  |
| Contexte de collecte | x | x |  |  |
| Méthode de collecte | x | x |  |  |
| Fréquence de mise à jour | x | x |  |  |
| Commentaires | x | x |  |  |
| **Données associées** | - | - | - | - |
| Table des données |  |  |  | x |
| **Conditions d'accès et d'utilisation** | - | - | - | - |
| Licence | x | x | x | x |
| Description | x | x | x | x |
| **Limitations** | - | - | - | - |
| Type | x | x | x | x |
| Restriction | x | x | x | x |
| Directive | x | x | x | x |
| Description | x | x | x | x |
| **Attriuts** | - | - | - | - |
| Table d'attributs | x | x |  |  |
| **Informations techniques** | - | - | - | - |
| Système de coordonnées | x | x |  |  |
| Echelle | x | x |  |  |
| Résolution | x | x |  |  |
| Nom de la couche | x | x |  |  |
| Format | x | x | x | x |
| **Qualité** | - | - | - | - |
| Specifications | x | x | x | x |
| **Contacts** | - | - | - | - |
| Contact | x | x | x | x |

## Export (XML, Impression)

### Téléchargement des métadonnées en pdf

Il est possible de générer un pdf contenant les métadonnées pour l'imprimer directement depuis l'OpenCatalog, en cliquant sur le bouton imprimer.

Ce pdf reprend toutes les métadonnées disponibles au moment de l'impression.

### Téléchargement au format XML

Il est possible de télécharger la fiche de métadonnée au format XML ISO 19139.

![Téléchargement de la métadonnée au format PDF et XML](/assets/usage/download_pdf_xml.png)

## Exploitation des services

Les conditions d'exploitation sont présentées dans la partie [Prérequis](/prerequisites.md).

### Visualisation dans l'OpenCatalog

Les données pouvant être visualisées peuvent être filtrées par l'action Visualisation dans le module de recherche ou le critère de recherche ```q=action:view``` directement dans l'URL.

Des liens de visualisation sont générés pour tous les services respectant les conditions d'exploitation.

![Visualisation services](/assets/usage/view.PNG)

Pour les Feature Services, l'affichage des informations sémantiques d'une géométrie est possible dans un pop-up au click sur cette géométrie.

![Affichage informations sémantiques](/assets/usage/semanticInfos.PNG)

### Extraction dynamique dans l'OpenCatalog

De même, l'extraction est possible pour tous les Feature Services respectant les conditions d'exploitation.

![Extraire](/assets/usage/extract.png)

Selon les capacités du serveur associé, l'OpenCatalog génère un formulaire d'extraction automatisée. Le formulaire propose alors l'extraction vers tous les formats et tous les systèmes de coordonnées disponibles pour la couche concernée.

![Formulaire d'extraction](/assets/usage/extractionModal.PNG)
