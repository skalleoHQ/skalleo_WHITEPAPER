# Skalleo blockchain



 

Une santé sécurisée, par tous pour tous. 

REMARQUE : Ce document est en cours d’élaboration. S’il vous plaît vérifier régulièrement pour les mises à jour ! 

 

### Table des matières 

Motivation 

Fonctionnement 

Qu’est-ce que Lisk ? 

Principes de conception 

Consensus et quorum du validateur 

Preuve d’enjeu déléguée 

Quorum du valideur 

Sécurité et finalité 

Récompense 

Plan économique des jetons 

Fonds d’amorçage 

Sécurité des données 

Perspectives  

 

## Motivation  

L’envie de rendre la santé accessible quelle que soit la situation géographique et de sécuriser le secteur sanitaire à travers le monde nous ont conduit à créer la blockchain skalleo.  

Celle-ci en partenariat avec chaque gouvernement, permettra à chaque citoyen de se soigner partout dans le monde d’une manière simple et sûre.   

Un manque de transparence pénalise aujourd’hui énormément le secteur sanitaire. Ainsi nous décidons de réparer les cassures qui adviennent tout au long des processus sanitaires en mettant en exergue la transparence des données. 

Notre seconde mission sera de mettre en place des structures sociales de santé qui fidéliseront les adhérents de SB. Comment ? 

A long terme, nous mettrons en place des centres de santé en accord avec chaque gouvernement. Et ceci permettra de réduire la charge à payer des citoyens.  

 

## Fonctionnement  

Alice a décidé de se rendre au Sénégal pour des raisons personnelles. Une fois sur place, Alice est malade et décide de trouver un médecin.  

Elle se demande comment trouver un bon médecin et sérieux ! 

Aucun problème, elle trouve un médecin enregistré sur skalleo qui pourra si besoin vérifier ses antécédents médicaux, se fait ausculter et reçoit son ordonnance. Son dossier médical est automatiquement mis à jour dans la base de données de son état. 

Elle se demande encore comment ne pas se faire arnaquer !  

Le paiement s’effectue automatiquement grâce au pool de solidarité du pays d’origine de Alice et le professionnel est payé au tarif fixé par l’état sénégalais.   

Mais comment trouver un pharmacien sérieux et ne pas recevoir de faux médicaments ! 

Elle trouve une pharmacie enregistrée sur skalleo, qui accède à l’ordonnance qu’elle vient de recevoir. Les médicaments émis sont ceux dont le numéro de série se trouve dans les données de l’état sénégalais. Le pool de solidarité de Alice sera débité du tarif fixé par l’état sénégalais et le professionnel est crédité de ce montant. 

Ce projet fera ses débuts grâce à Lisk et si nécessaire nous concentrerons nos efforts sur la création d’une blockchain propre ultérieurement. 

 

## Qu’est-ce que Lisk ?  

Les développeurs peuvent construire, publier, partager et monétiser leurs dApps (applications décentralisées) sur la blockchain Lisk. Celles-ci sont développées avec du code JavaScript. 

Chaque application décentralisée (dApp) fonctionne sur sa propre sidechain. C’est-à-dire que ces applications ne sont pas intégrées à la blockchain Lisk mais qu'elles gravitent autour. La blockchain principale de Lisk ne sera donc pas impactée directement par les sidechains. Les sidechains sont donc des blockchains autonomes qui sont dissociées de la blockchain principale Lisk.  

Les spécificités des sidechains de Lisk peuvent être adaptées et optimisées en fonction des besoins d'une blockchain. Si un hardfork est nécessaire à cause d’un bug découvert dans la sidechain, seule cette dernière devra être modifiée. Il n’y aura donc aucun impact sur la mainchain et les autres sidechains.  

 

## Principes de conception 

Après la création de la blockchain dans l’écosystème Lisk, deux blockchains fonctionneront côte à côte pour fournir des services différents. La nouvelle chaîne s’appellera << skalleo blockchain >> (abréviation de << SB >> pour les sections ci-dessous), tandis que le réseau principal restera nommé Lisk. 

Voici les principes de conception de SB :  

Blockchain autonome : techniquement, SB est une blockchain autonome, au lieu d’une solution de couche 2. La plupart des fonctions techniques et commerciales fondamentales de SB devraient être autonomes afin qu’elles puissent bien fonctionner même si Lisk s’arrêtait pendant une courte période. 

Compatibilité Lisk : pour ne pas enfermer son réseau, SB choisit d’être compatible avec le réseau principal Lisk existant. Cela signifie que la plupart des dApps, des composants de l’écosystème et des outils fonctionneront avec SB et nécessiteront zéro ou un minimum de modifications. 

Le protocole de consensus du staking et la gouvernance : le consensus basé sur le forgeage délégué est plus respectueux envers l’environnement et laisse une option plus flexible à la gouvernance communautaire. Ce système devrait permettre de meilleures performances sur le réseau par rapport au système proof-of-work basé sur le minage, c’est à dire un temps de forgeage de bloc plus rapide et une capacité de transaction plus élevée. 

Communication inter-chaînes native : SB prévoit de mettre un support natif afin de permettre la communication inter-chaînes avec des stables coins comme Tether.... Le protocole de communication doit être bidirectionnel, décentralisé et sans faille. Il se concentrera sur le déplacement d’actifs numériques par exemple entre SB et Tether, USDC... 

 

## Consensus et quorum du validateur  

Basé sur les principes de conception, le protocole de consensus de SB est d’atteindre les objectifs suivants :  

Le temps de blocage devrait être plus court que le réseau Lisk, par exemple 5 secondes ou même plus court afin de couvrir toutes les transactions partout dans le monde. 

Il faut un temps limité pour confirmer la finalité des transactions, par exemple environ 1 min ou moins. 

Il n’y a pas d’inflation du jeton natif SKA : la récompense de bloc est collectée à partir des frais de forgeage, et elle sera payée en LSK (monnaie de Lisk). 

La compatibilité avec le système de stables coins autant que possible. 

Le jeton SKA représentera la capitalisation de la blockchain skalleo et permettra de gouverner. 

### Preuve d’enjeu déléguée  

Bien que la preuve de travail (PoW) ait été reconnue comme un mécanisme pratique pour mettre en œuvre un réseau décentralisé, elle n’est pas durable pour l’environnement et nécessite également un grand nombre de participants pour maintenir la sécurité. 

De ce fait, nous choisirons d’utiliser la preuve d’enjeu déléguée (DPoS) qui est le consensus de base de Lisk. Considérant que l’intérêt commun doit primer sur l’intérêt personnel, les détenteurs de pool de solidarité seront élus d’office comme les forgeurs. Ce qui signifie que chaque état sera un délégué (forgeur) et veillera à la sécurité de la blockchain. 

SB propose ici de modifier le DPoS :  

Les blocs sont produits par un ensemble limité de valideurs. 

Les valideurs se relaient pour produire des blocs de manière PoA c’est à dire seul les élus pourront forger des blocs. 

Les valideurs seront d’office les états détenteurs de pool de solidarité. 

### Quorum du valideur  

Au stade de la genèse, uniquement les pools de solidarité disponibles s’exécuteront en tant que valideur initial. Une fois la blockchain commencée, n’importe quel état peut se joindre en tant que valideur. 

Lors de la production d’autres blocs, les valideurs SB existants vérifient si un message est relayé périodiquement sur SB. Si c’est le cas, ils mettront à jour le valideur défini après une période d’époque, c’est-à-dire un nombre prédéfini de temps de blocage. Par exemple, si SB produit un bloc toutes les 5 secondes et que la période d’époque est de 240 blocs, l’ensemble de valideurs actuel vérifiera et mettra à jour le cercle de valideurs pour l’époque suivante en 24 h (1440 minutes). 

Sécurité et finalité  

La sécurité de la blockchain dépendra entièrement des valideurs (états) et ceux-ci ne mettront pas en péril sa transparence au risque de perdre entièrement leur liquidité. 

Naturellement s’il y a N états adhérents donc N valideurs, les nœuds de la blockchain sont tous sains car leurs valideurs mettent en jeu leur fonds de solidarité. 

### Récompense  

Tous les valideurs de SB seront récompensés par des frais de forgeage en LSK. Comme LSK est un jeton inflationniste, il y aura des récompenses minières comme ce que le réseau Bitcoin et Ethereum génèrent, et les frais de transaction sont la principale récompense pour le pool de solidarité mondiale ou notre rémunération. 

Ceci permettra de prôner l’intérêt commun car les récompenses minières contribueront aux fonds de solidarité de l’état valideur.  

Les frais de transaction proviendront d’une portion des paiements des professionnels et assureront le fonctionnement de skalleo que ce soit la rémunération du personnel, l’ouverture de centre de santé à œuvres sociales etc... Ou encore à financer un pool de solidarité mondiale pour des œuvres caritatives. 

 

## Plan économique des jetons  

SKA et LSK ne partagent pas le même univers de jetons. Celui-ci définit : 

Les jetons LSK s’utiliseront dans la blockchain afin de rémunérer les forgeurs. 

Les jetons LSK et les stables coins devront être convertibles de manière bidirectionnelle et pourront circuler sur le réseau skalleo.  

Les stables coins s’utiliseront pour payer les professionnels de santé. 

Le jeton SKA sera déflationniste et capitalisera la SB. 

### Fonds d’amorçage  

Au début de la blockchain, chaque contribuable est libre d’acheter des LSK ou des stables coins pour n’importe quelle raison, que ce soit pour faire des dons aux pools de solidarité, remercier un professionnel etc... 

Quant aux pools de solidarité, il sera nécessaire d’amorcer leur compteur avec un montant minimal et crédible en stable coins.  

 

## Sécurité des données  

SB renforcera la sécurité de ses données en limitant l’interopérabilité avec d’autres applications. Comme cité plus haut, SB choisit d’être interopérable avec le réseau principal Lisk. 

Cependant ne seront admises que les applications à finalité identique à SB afin de réduire au mieux tous risques pouvant porter atteinte à SB et ses utilisateurs.  

Les données santé seront sauvegardés en plugin ceci permettra de stocker ces données uniquement dans quelques nœuds. Contrairement aux données santé, les comptes patients, professionnels et pools de solidarité seront enregistrés en état dans la blockchain, car celles-ci se trouvent au cœur des transactions à savoir (les transactions de soins transmis, les paiements à effectuer...) 

Ainsi les délégués seront en mesure de garder les données santé des patients puisqu’ils représentent les principaux garants de la blockchain. Quant aux professionnels et patients, leur accès à ces données est indispensable, puisqu’ils contribuent à l’élaboration de celles-ci.  

 

## Perspectives  

SB se fixe comme objectifs à court-terme :  

La connexion entre les jetons LSK et les stables coins. 

Le paiement des professionnels en stable coins. 

La possibilité de sauvegarder des stable coins dans les comptes professionnels et les pools de solidarité. 
