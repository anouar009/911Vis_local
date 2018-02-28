## Review d'un projet de data visualisation

Projet à analyser : [Visualisation des resultats du Baccalauréat 2016](https://github.com/ArnaudBru/ProjetBAC)

*to be continued*

### Description du problème 

La descritpion du problème est un peu vague. Il s'agit en effet de : *'Visualisation interactive des résultats du baccalauréat 2016 en France Métropolitaine dans les lycées d'enseignement général et technologique, au travers d'une carte choroplèthe'.* 

Si cette défiition du problème fait bien ressortir l'aspect géographique de la visualisation, on ne sait cependant pas à quel découpage géographique nous pouvons nous attendre :
* Région?
* Département?
* Académie?
* Ville?
* Lycée?

On ne sait ni précisément à quoi réfère le terme 'résultats'. S'agit-il :
* De taux de réussite?
* De nombre de diplômés?
* Du taux de mentions?

Ainsi le problème permet certes d'avoir une idée globale de la visualisation désirée mais il ne permet pas de cadrer précisément les éléments qui seront visualisés.

Après analyse de la proposition de design, il serait plus judicieux de poser le problème sous la forme : *Visualisation des disparités dans le taux de réussite au bac en fonction des départements, des filières et du type d'établissement?*


### Choix des visualisations

Les [design sheets proposées par l'équipe du projet BAC](https://github.com/ArnaudBru/ProjetBAC/blob/master/PROPOSAL.MD) permettent de préciser les éléments présents dans la visualisation. Il s'agit :
* Des taux de réussite  par département
* Des taux de réussite par type d'établissement
* Des taux de réussite par filière

La précision géographique sera limitée au département.

#### Carte choroplète

Cette visualisation semble naturelle pour des données organisées géographiquement et présentant une variable continue (i.e. le taux de réussite). C'est un choix judicieux.

On peut se demander cependant si le découpage géographique ne pourrait pas être mieux adapté. Au lieu de se limiter aux départements, on peut imaginer des niveaux de zoom différents :
* Au niveau de l'académie (difficile peut être d'en tracer les contours?)
* Au niveau des communes
* Au niveau des lycées (passage à des marqueurs discrets, trop fin peut être?)

En effet il est peu probeble que la visualisation soit assez fine au niveau des départements pour que ressortent de réelles différences

#### Sequences sunburns

Le choix de cet outil est très intéressant pour visualiser les disparités entre public/privé et filières. Il semble tout à fait adapté dans le cadre de cette visualisation.

Cependant il ne semble pas prévu de le lier avec le focus géographique (sélection d'un département), il n'affiche que les dispqrités au niveau national. Il pourrait être intéressant de le lier au ficus géographique.

#### Stacked bar chart

Cet outil de visualisation sera utilisé lors du focus géographique sur un département. Il permet de compléter en partie l'absence de focus sur le sequence sunburn en affichant les taux de réussite par filière au sein du département.

Il n'est pas incompatible avec la présence du sequence sunburn, même si ce dernier est modifié pour suivre le focus géographique. En effet le sequence sunburn montre surtout la disparité public/privé et le stacked bar chart la disparité entre filières.

#### Conclusion

Les visualisations semblent adaptées et judicieusement choisies pour visualiser le taux de réussite au BAC, en fonction des départements, des filières et du type de l'établissement. Il peut être intéressant cependant de définir plus finement les niveaux de découpage géographique possibles!

### Faisabilité du projet

Le projet semble tout à fait faisable. Les données ne sont pas volumineuses, elles sont structurées et les visualisations proposées sont réalistes.

### Autres remarques

*pas d'autres remarques*
