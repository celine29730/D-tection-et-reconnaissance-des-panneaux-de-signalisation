¶# Détection et reconnaissance des panneaux de signalisation

Objectif de l'étude: construire un modèle IA pour la détection et la reconnaissance des panneaux de signalisation sur les images et sur la vidéo.
Contexte du projet

Dans le monde de l'IA des grandes entreprises comme Tesla, Uber, Google, Mercedes-Benz, etc. travaillent sur des véhicules autonomes et des voitures autonomes. Pour atteindre la précision de cette technologie, les véhicules doivent être capables d'interpréter les panneaux de signalisation et de prendre des décisions en conséquence. Votre objectif est de construire un modèle qui permet de réaliser cette tâche.

Une interface graphique est demandée:

* Qui permet de détecter dans une image les panneaux de signalisation et les reconnaitre (Afficher le label en Français).
* Qui permet de détecter tous les panneaux dans une vidéo les reconnaitre et les afficher avec leurs labels.

Description des fichiers

L'ensemble de données que nous allons utiliser pour former notre propre classificateur de panneaux de signalisation personnalisé est un ensemble de données qui comprend 43 classes de panneaux de signalisation et près de 50 000 images.

Il existe plusieurs types de panneaux de signalisation tels que les limitations de vitesse, es feux de signalisation , tourner à gauche ou à droite, pas de passage de véhicules lourds, etc. La classification des panneaux de signalisation est le processus d'identification de la classe à laquelle appartient un panneau de signalisation.

La définition de nos 43 classes de panneaux se trouve dans le répertoire "Meta" où figure nos 43 panneaux type. le fichier Meta.csv reprend ces 43 images ainsi que toutes les caractéristiques individuelles des panneaux(image, Numéro de classe, taille,couleur...).

Notre jeu de données est déjà fractionné en jeu d'apprentissage et de test. Les images ainsi que leur caractéristiques propres figurent respectivement dans les fichiers Train.csv et Test.csv. L'ensemble de données a un dossier train qui contient des images à l'intérieur de chaque classe et un dossier de test que nous utiliserons pour tester notre modèle.

Dans notre projet, nous allons créer un modèle de réseau neuronal profond qui peut classer les panneaux de signalisation présents dans l'image dans différentes catégories. Avec ce modèle, nous sommes capables de lire et de comprendre les panneaux de signalisation qui sont une tâche très importante pour tous les véhicules autonomes.



Suite à notre étude,nous avons bien classé le classificateur des panneaux de signalisation avec une précision de 95% et avons également visualisé comment notre précision et notre perte changent avec le temps, ce qui est plutôt bon à partir d'un simple modèle CNN.

L'interface graphique rélisé permet de bien classer nos panneaux avec le libéllé qui convient:
[image4](https://github.com/celine29730/D-tection-et-reconnaissance-des-panneaux-de-signalisation/blob/main/image%204.png)

Il suffit pour cela de cliquer sur **UPLOAD an image** afin de télécharger une image.

[image1](https://github.com/celine29730/D-tection-et-reconnaissance-des-panneaux-de-signalisation/blob/main/image1.png)

puis d'appuyer sur **CLASSIFY** pour avoir le libéllé qui correspond à l'image.

[image2](https://github.com/celine29730/D-tection-et-reconnaissance-des-panneaux-de-signalisation/blob/main/image%202.png)
