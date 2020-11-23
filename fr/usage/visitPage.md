# Consulter une page
## Champs
Les champs disponibles dépendent du type de la donnée. Pour chaque type de donnée, tous les champs remplissables depuis l'interfaction d'administration APP sont disponibles.

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
| **Attriuts** | - | - | - | - |
| Table d'attributs | x | x |  |  |

## Export (XML, Impression)
### Téléchargement au format XML
### Téléchargement des métadonnées en pdf
Il est possible de générer un pdf contenant les métadonnées pour l'imprimer directement depuis l'OpenCatalog, en cliquant sur le bouton imprimer.

Ce pdf reprend toutes les metadonnées disponibles au moment de l'impression.

## Exploitation des services
Les conditions d'exploitation sont présentées dans la partie Prérequis.
### Visualisation dans l'OpenCatalog
Les données pouvant être visualisées peuvent être filtrées par l'action Visualisation dans le module de recherche ou le critère de recherche ```q=action:view``` directement dans l'URL.

Des liens de visualisation sont générés pour tous les services respectant les conditions d'exploitation.

![Visualisation services](/assets/usage/view.PNG)

Pour les Feature Services, l'affichage des informations sémantiques d'une géométrie est possible dans un pop-up au click sur cette géométrie.

![Affichage informations sémantiques](/assets/usage/semanticInfos.PNG)

### Extraction dynamique dans l'OpenCatalog
De même, l'extraction est possible pour tous les Feature Services respectant les conditions d'exploitation.

![Extraire](/assets/usage/extract.PNG)

Selon les capacités du serveur associé, OpenCatalog génère un formulaire d'extraction automatisée. Le formulaire propose alors l'extraction en tous les formats d'intérêt disponibles et tous les systèmes de coordonnées disponibles pour la couche.

![Formulaire d'extraction](/assets/usage/extractionModal.PNG)
