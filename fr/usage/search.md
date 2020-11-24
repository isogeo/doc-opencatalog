# Recherche une donnée
## Filtres
Deux outils permettent de filter les données :
* Un module de filtre
* Une barre de recherche

### Module de filtre

Les filtres sont appliqués selon un critère de 'et strict', c'est à dire que tous les critères demandés doivent être respectés pour que la donnée soit retournée.

![Module de filtre](/assets/usage/filterWidget.PNG)

### Barre de recherche

Une barre de recherche est disponible.
![Barre de recherche](/assets/usage/researchBar.PNG)

#### Utilisation : Autocompletion

#### Utilisation : Nomenclature de tag
Il est également possible d'utiliser directement la nomenclature de tag isogeo pour requêter.
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

Par exemple, rechercher la chaîne de caractère `coordinate-system:2154 action:download` revient à selectionner le système de coordonnées Lambert-93 et l'action Télécharger.

#### Particularités
Cette nomenclature est notamment utilisée dans l'URL lorsqu'une requête est lancée.

####
De la même manière que le module de filtre, les données sont retournées si tous les critères sont respectés.

## Tri
Il est possible de trier les données disponibles selon deux critères :
* le sens du tri : tri ascendant ou descendant
* l'object du tri : tri par petinence (tri par défaut), tri alphabétique, tri par date de mise à jour de la métadonnées et tri par date de mise à jour de la donnée
