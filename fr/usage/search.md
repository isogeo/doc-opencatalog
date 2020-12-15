---
description: Description de la page de recherche de l'OpenCatalog
---

# Rechercher une fiche de métadonnée

L'OpenCatalog exploite toute la puissance du moteur de recherche Isogeo. L'OpenCatalog dispose d'un widget de filtres et d'une barre de recherche avec autocomplétion. La combinaison des deux permet de retrouver facilement les fiches de métadonnées souhaitées.

## Filtres

Deux outils permettent donc de filter les données :

* Un module de filtre
* Une barre de recherche

### Module de filtre

Il est possible de filtrer les données selon les critères suivants :

* Un texte au choix qui doit être trouvé dans les champs de métadonnées suivants : titre, nom, résumé, nom de la couche associée, nom des attributs de la table attributaire
* le propriétaire si des catalogues de plusieurs groupes de travail sont partagés,
* un ou plusieurs mots-clés,
* le type de la donnée,
* le format de la donnée,
* le système de coordonnées,
* un ou plusieurs thèmes Inspire,
* une ou plusieurs actions possibles (téléchargement, visualisation, autre),
* une ou plusieurs licences associées,
* un ou plusieurs contacts.

À chaque sélection d'un filtre, le nombre de résultats et les valeurs possibles des autres filtres sont rapidement mis à jour. Si un nouveau filtre est renseigné et qu'une seule valeur d'un autre filtre est disponible, elle est automatiquement sélectionné.

![Module de filtre](/assets/usage/filterWidget.PNG)

> Les filtres sont appliqués selon un opérateur d'intersection "*et*", c'est à dire que tous les critères demandés doivent être respectés pour que la donnée soit retournée.

### Barre de recherche

Une barre de recherche avec autocomplétion est utilisable, il suffit d'écrire puis de sélectionner le champ proposé dans la liste en cliquant sur `Entrée`.

![Barre de recherche](/assets/usage/researchBar.png)

#### Utilisation avancée : Nomenclature des champs

Il est également possible d'utiliser directement la nomenclature des champs Isogeo tels qu'ils sont décrits dans l'API pour rechercher une donnée.

| Champs | Nomenclature de recherche |
|:------:|:----------------------------------:|
| Propriétaire | `owner:` suivi de l'id du propriétaire |
| Mots-clefs | `keyword:isogeo` suivi du tag correspond au mot-clef |
| Type | `type:` suivi des tags d'un des quatre types |
| Format | `format:` suivi du tag du format souhaité |
| Système de coordonnées | `coordinate-system:`suivi du tag correspondant au système de coordonnées |
| Thèmes inspire | `keyword:inspire-theme:` suivi du tag correspondant au thème inspire |
| Action | `action:` suivi du tag correspondant à l'action souhaitée |
| Licence | `license:` suivi de l'id de la license |
| Contact | `contact:` ou  `contact:group:` en fonction du type de contact suivi de l'id du contact |

Par exemple, rechercher la chaîne de caractère `coordinate-system:2154 action:download` revient à sélectionner le système de coordonnées `Lambert-93` et l'action `Télécharger`.

> NB : Cette nomenclature est notamment utilisée dans l'URL lorsqu'une requête est lancée.

#### Autre

* De la même manière que le module de filtre, les données sont retournées si tous les critères sont respectés.
* Attention : Contrairement au module de filtre, la valeur "Non renseigné" est proposée pour tous les champs peu importe l'existante de données correspondant à ce critère, tant qu'aucune valeur autre pour ce champs est sélectionnée

## Tri

Il est possible de trier les données disponibles selon deux critères :

* le sens du tri : tri ascendant ou descendant
* l'object du tri : tri par pertinence (tri par défaut), tri alphabétique, tri par date de mise à jour de la métadonnées et tri par date de mise à jour de la donnée
