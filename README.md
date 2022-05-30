# architectures-de-topologie-reseau

### Les réseaux LAN sont conçues sous la base des 3 niveaux ou couches suivantes :
* Accès
* Distribution
* Cœur

## Types d'architectures
### Architecture 2 tier
* Cœur et Distrib sont combinées.
* Les commutateurs du haut exécutent des fonctionnalités de niveau de distribution en fournissant une connectivité pour les commutateurs de couche d’accès.

![image](https://user-images.githubusercontent.com/83721477/170944499-8c6866ea-e79f-4c0d-a181-a4cc8c9a453d.png)

### Architecture 3 tier

![image](https://user-images.githubusercontent.com/83721477/170945036-54f53a37-a455-4d79-9e5e-fdedfa96cad9.png)

À mesure que le nombre de commutateurs de distribution augmente, il est difficile d’établir une connectivité maillée complète dans ce cas on est obligé de faire une architecture 3 tier.<br>
Cela consiste à mettre en œuvre un ensemble dédié de périphériques de base(niveau coeur), de sorte que chaque commutateur de distribution soit connecter à chacun d’eux

### Architecture Leaf-Spine
L’architecture Leaf-Spine représente une `topologie de réseau de Datacenter` de plus en plus populaire.<br>
Elle consiste en deux niveaux composés de commutateurs « feuilles » (Leaf) et de commutateurs « troncs » (Spine).<br>
Chaque périphérique d’une couche se connecte à chaque périphérique d’une autre couche. Aucun lien direct n’existe entre les appareils situés sur la même couche.

![image](https://user-images.githubusercontent.com/83721477/170945833-03a0e52e-c39e-402b-a181-04b309bf8822.png)

### Architecture SOHO (Small Office/ Home Office)
Les réseaux SOHO (petits bureaux / bureaux à domicile) sont généralement conçus pour répondre à des exigences telles que la réduction du nombre d’appareils et la minimisation de la complexité de la configuration tout en maintenant la sécurité au niveau de l’entreprise.

![image](https://user-images.githubusercontent.com/83721477/170946493-15d04a4e-31dc-45a6-ac77-53372b66a2d8.png)

