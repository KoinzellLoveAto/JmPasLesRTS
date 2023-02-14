## **Cahier des charges**

HUVA est un jeu typé **RTS** dans lequel vous devrez survivre à de multiple vague pendant un système jour/nuit. Ce jeu est réalisé avec **Unreal Engine 5**


## **Univers**
Utilisation du pack Sci-Fi pour la mise en place de l'univers : https://syntystore.com/collections/frontpage/products/polygon-sci-fi-worlds

## **Source Inspiration**
![AgeOfEmpireII](https://www.biendebuter.net/wp-content/uploads/2014/10/23081053091comparo.jpg)
![TheyAreBillions](ImageRepo/BillionsIcon.png)

## **Scénario Tutoriel, Guidage Joueur**
Le village a été ravagé durant la dernière lune, tous les bâtiments ont été réduit en poussière sous les coups des adversaires, au lever du soleil
Ces derniers partent à la vue du soleil et des renforts alliés arrivant malheureusement trop tard. Pour ce début de jeu le joueur pourra assister à une petite mise
En scène expliqué au-dessus, lorsque que les adversaires sortent du village le joueur pourra prendre contrôle des unités renforts et sera convié a reconstruire
Le village (un des bâtiments pouvant être reconstruit du village). 

Le jeu sera découpé en deux partie, une en jour et une autre de nuit, il sera expliqué a travers de boite de dialogue ou texte affiché sur l'HUD les étapes à suivre durant ce cycle.

La période en jour, le joueur devra construire, dépenser ces ressources pour créer des unités ou réparer des bâtiments permettant la création d'unité spéciale

La période de nuit consiste à survivre à de multiple vagues venant de différent coté du village, chaque adversaire éliminé permettra de gagner de l'argent.

Lorsque toutes les nuits ont été effectué et que le joueur a survécu il sera accueilli avec un écran de remerciement pour avoir joué a la démo du jeu HUVA

**Étapes : ** (Avant chaque étape le jeu sera mis en pause)
 - Montrer le système de sélection par unité ou pour un ensemble avec la sélection multiple en rectangle
 - Cliquer sur un bâtiment avec une ou plusieurs unités sélectionnées le bâtiment principal pour le reconstruire ce qui permet de créer des simples IA
 - Ensuite sélectionner le bâtiment pour créer d'autre IA
 - Construire le bâtiment des troupes d'attaques
 - Générer des troupes d'attaques
 - Placer les troupes pour défendre
 - Reconstruire une tour de défense
 - La Nuit tombe
 - Début de la vague et montrer la sélection d'unité pour attaquer une unité ennemie précisément, ou la plus proche, celle qui à le plus de PV, celle qui est la plus faible, ...
 - Continuer jusqu'à la 10ème vague
 - FIN (Ou mort prématuré : Plus d'unité et de bâtiment en bonne état)

## **Entités**
**Alliés**
 - Humain builder
 - Humain fighter

**Ennemies**
 - Tank : Monstre qui attaque au corps à corps avec beaucoup de PV et marche lentement
 - Shooter : Monstre qui attaque à distance avec peu de PV

## **Schéma Map**
![Map](ImageRepo/Map.png)

## **Mécanique principale avec IA Employé**
1. Mécanique Construction/Réparation de bâtiments
	- Création d'unité
	- Gain d'argent
	- Création de tour
	- Gain Emplacement d'espace
2. Mécanique Achat
	- Unité
	- Bâtiments
3. Mécanique Unité Allié
	- Flocking pour se répartir sur une zone
	- AI Utility pour déterminer quelle unité à attaqué
	- Behaviour Tree
	- Entité 
4. Mécanique Unité Ennemie
	- Behaviour Tree
5. Mécanique Vague / Spawner
	- Fait apparaitre des adversaires
	- Choisi le point d'arrivée du Village (Ouest, Nord, Est)



