# architectures-de-topologie-reseau

### Les réseaux LAN sont conçues sous la base des 3 niveaux ou couches suivantes :
* Accès
* Distribution
* Cœur


### Couche d'accès

* C'est la couche la plus proche des utilisateurs finaux.
* Les utilisateurs sont connectés à ces commutateurs.
* Les politiques d'accès au réseau, les mécanismes de sécurité de couche 2 tels que la sécurité des ports (port-security) sont utilisés.
* Les mécanismes de prévention de boucle de couche 2 tels que STP, RSTP, PVST, MST sont utilisés dans cette couche.
* Les VLAN sont une autre technologie importante et la plus utilisée dans cette couche.

### Couche de distribution
Le rôle de cette couche a pour rôle de filtrer, de router, d’autoriser ou non les paquets.

* Bridge de la couche d'accès et de la couche coeur.
* Agrégation de tous les commutateurs d'accès.
* Au lieu de commutateurs L2, des commutateurs L3 sont utilisés dans la couche de distribution.
* La redondance est utilisée dans cette couche pour surmonter le point de défaillance unique. 
* Les politiques de distribution sont également utilisées dans cette couche.

### Couche Coeur

La couche Coeur est également connue sous le nom de Backbone Network.<br>
Le rôle consiste à relier entre eux les différents segments  d’un réseau à savoir : les sites distants, les réseaux locaux (LANs) ou les étages de l’immeuble d’une société.

* Les protocoles de routage sont utilisés dans cette couche
* Fournir un routage entre eux et la couche de distribution.
* Mise en place de dispositifs centraux redondants pour surmonter le point de défaillance unique.

 

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

### Architectures WAN

Les principales topologies utilisées sur les WAN sont indiquées ci-dessous :

* Point-to-Point
* Hub and Spoke
* Full Mesh
* Dual-Homed

