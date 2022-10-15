# Deep Learning pour la classification de graphes créés à partir de la BDD Corine Land Cover

## Données

[Corine Land Cover](https://land.copernicus.eu/pan-european/corine-land-cover)

## Objectif

Classification du territoire européen à partir de graphes

## Méthode proposée

### Subdivision bas niveau du territoire européen

* Utiliser la [base de données GISCO](https://ec.europa.eu/eurostat/fr/web/gisco/geodata/reference-data/administrative-units-statistical-units/communes) pour sélectionner des communes d'Europe
* Créer un graphe par commune grâce à la BDD Corine Land Cover

### Classification de graphes

* Réduire la dimension des graphes en utilisant des techniques de plongement de graphes (embedding)
* Classer les vecteurs obtenus en entraînant différents modèles de Deep Learning (MLP, CNN)
* [Etat de l'art](https://arxiv.org/pdf/1709.07604.pdf?ref=https://githubhelp.com)
* [graph2vec](https://arxiv.org/pdf/1707.05005.pdf)
    
