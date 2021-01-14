# FAQ : Explication des erreurs de visualisation

Que signifient les différentes erreurs qui peuvent se produire lors de la visualisation de flux cartographique ?

* _Impossible de charger les données_ : Aucune tuile n'a pu être récupérée.
* _Attention : Il peut manquer des tuiles_ : Certaines tuiles demandées n'ont pas pu être récupérées.
* _Impossible de visualiser les donnée_ : La récupération des données n'a pas abouti. Le serveur est probablement indisponible ou renvoit une erreur. 
* _La version du gml en sortie n'est pas supportée_ : Le gml3 ou le geojson n'est pas un format de sortie supporté par le serveur cartographique en question. Or un de ces deux formats doient être disponibles pour permettre l'affichage sur l'OpenCatalog. 
* _Des données n'ont pas de géométrie_ : Des entités récupérées depuis le serveur n'ont pas de géométrie associée. La couche n'est alors pas ou que partiellement affichée.
* _La couche a mis trop longtemps à charger_ : La requête n'a pas abouti au bout du temps maximal consacré à la tâche. 
