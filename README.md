# P-T

# **Bienvenue dans ce github !**

L’objectif est d’assurer une victoire de P&T à la coupe de France de robotique. Les choses sont mises au clair, vous saurez à quoi vous attendre ici : l’excellence, ou rien du tout.

## Prérequis:
Il faut connaître la coupe de France de robotique, et le genre d’actions qui doivent être effectuées par le robot. Pour cela, cf leur site et les règlements des différentes coupes. Ici en exemple, le règlement 2024:

https://www.coupederobotique.fr/edition-2024/le-concours/reglement-2024/ 

## Principe:
Voici comment se partagent les objectifs. Nous allons traiter de toute la partie caméra / IA : caméra embarquée, caméra sur perche, IA de décision, communication entre l'ordinateur et la Raspberry Pi. Voici le matériel que j’utilise ici: 

* Une Raspberry Pi 4 Model B
  
* Une Raspberry Pi Camera Rev 22
  
* Une webcam (toute caméra pouvant être branchée à un ordinateur peut faire l’affaire)
  
* Un ordinateur avec Python (Puissance de calcul considérée comme illimitée)



### Ce github est découpé en trois parties: 
1)  Caméra embarquée / Raspberry Pi
2)  Webcam / Ordinateur, Communication avec la Raspberry pi
3)  IA décisionnelle

Je vais détailler un peu chaque partie ci-dessous.

## CAMÉRA EMBARQUÉE / RASPBERRY PI

L’objectif est de récupérer les données de la caméra, pour reconnaître et situer les éléments de la table de jeu par rapport au robot. On se penchera donc ici sur de la reconnaissance d’objets à partir d’une Raspberry Pi et de sa caméra.

## WEBCAM / ORDINATEUR, COMMUNICATION AVEC LA RASPBERRY PI

Les données de la Webcam seront récupérées sur l’ordinateur. Cette Webcam aura une vision sur toute la table de jeu. L’objectif est de récupérer la position du robot dans les coordonnées de la table à partir de ces informations. Le robot aura au-dessus du châssis un QR code; on s’attardera ainsi ici à faire 1) du tracking de QR code et de la reconnaissance des objets importants de la table de jeu et 2) de la transposition du système de coordonnées dans le repère de la caméra à celui de la table.
Dans un second temps, l’objectif est de communiquer avec la Raspberry Pi afin de récupérer ses données et d’envoyer les siennes.

## IA DÉCISIONNELLE

Après ces deux étapes effectuées et en fonction des objectifs à remplir par le robot, il faudra être en mesure de prendre les bonnes décisions. Une IA sera utilisée dans ce but, qui utilise tous ces paramètres pour décider de quelle action est la plus optimale en un moment donné.


# Conclusion: 

Au travail, on a du boulot...
