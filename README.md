    # DL-BDgéographiques-Massimo-VENUTI

## Données
* [RPG](https://geoservices.ign.fr/rpg#telechargement)
* [Corine Land Cover](https://land.copernicus.eu/pan-european/corine-land-cover)

## Objectif : classification hiérarchique non-supervisée du territoire français à partir de graphes
* Construire un graphe par commune avec sa zone Corine Land Cover -> regroupement des communes qui se ressemblent

## Méthode proposée
### Subdivision bas niveau du territoire français
* Utiliser la [base de données des communes de France](https://www.data.gouv.fr/fr/datasets/r/0e117c06-248f-45e5-8945-0e79d9136165) pour sélectionner environ 5000 communes ayant une superficie proche
* Créer un graphe par commune grâce à la BD Corine Land Cover

### Classification de graphes
* Réduire la dimension des graphes en utilisant des techniques de plongement de graphes (embedding) pour les classer (attribuer automatiquement un label de classe à chaque graphe pour) grâce à la détermination d'une valeur de similarité entre paire de graphes
    - un [état de l'art](https://arxiv.org/pdf/1709.07604.pdf?ref=https://githubhelp.com) -> la partie 5.3.1 est un bon point de départ à creuser (aller sur [google scholar](https://scholar.google.fr/), pour chaque article de la section, cliquer sur 'Cité ... fois' en dessous de l'article afin de découvrir les articles plus récents en lien avec l'article recherché.
    - exemple de méthode plus récente que l'état de l'art : [graph2vec](https://arxiv.org/pdf/1707.05005.pdf)
    - Faire de la bibliographie : pour chaque article lu, noter sa référence ainsi que les avantages et inconvénients pour ce qu'on veut faire
    
