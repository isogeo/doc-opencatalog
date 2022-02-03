---
description: Ajouter les métadonnées de l'OpenCatalog aux couches publiées avec GEO Générateur de Business Geographic
---

# Ajouter les métadonnées aux couches dans GEO Générateur

La solution `GEO Générateur` de Business Geographic permet de publier des cartographies interactives contenant différentes sources de données géographiques. Lors de l'intégration d'une donnée dans `GEO Générateur`, il est possible d'intégrer une url qui pointe vers la métadonnée. Pour remplir ce champ, il suffit de récupérer l'url de l'Opencatalog de la fiche de métadonnées correspondante en mode `?lock` (cf. [Intégrer une page unique en mode lock](/usage/generate.md#lock)).

1. Ouvrir `GEO Générateur` ;
2. Dans la partie `Données`, on retrouve la liste des tables ou des fonds de plan ;
![Afficher les données](/assets/appendices/geo_tables.jpg)
3. Ajouter une table ou sélectionner une table ;
4. Ouvrir l'onglet `Infos` ;
![Onglet Infos de la table](/assets/appendices/geo_edit_table.jpg)
5. Cliquer sur `Editer` ;
6. Dans `URL de métadonnées`, coller l'url de la métadonnée en mode `?lock`
Exemple : `https://open.isogeo.com/s/8d491301f61249139918e3710cd39eb7/wak8OBU2hQX6F6rtIe3fWiRCvzFH0/r/10383c7f97ba470fbbffdd46d3e99308?lock`
![Onglet Infos de la table](/assets/appendices/geo_edit_table_metadata.jpg)
7. Ajouter la donnée à une carte et lui affecter un style au besoin ;
8. Visualiser la carte, on retrouve le lien dans le menu `Carte` depuis le bouton en forme d'étiquette ;
![Legende de la carte GEO](/assets/appendices/geo_map_legend.jpg)
9. Cliquer sur `Afficher les métadonnées` ;
![Afficher les métadonnées](/assets/appendices/geo_map_legend_show_metadata.jpg)
10. Une fenêtre s'ouvre et la fiche de l'OpenCatalog s'affiche.
![Fenêtre de visualisation de la métadonnée de l'OpenCatalog](/assets/appendices/geo_window_with_metadata.jpg)
11. Vous pouvez, bien sûr, procéder de la même manière avec un fond de plan ou une orthophoto.
