Projet Transfer Learning pour la détection de port de masque
Ce projet a pour objectif d'appliquer la technique du Transfer Learning sur une base de données d'images afin de développer un modèle de machine learning capable de déterminer si une personne porte un masque facial ou non. Le projet sera réalisé en utilisant Google Colab (https://colab.research.google.com/?hl=fr) pour l'apprentissage du modèle.

Contexte du projet
Le projet est guidé par plusieurs défis techniques :

1. Manipulation d'Images
Il est essentiel de maîtriser la manipulation des images, notamment le chargement, la redimensionnement, et la préparation des images pour les rendre compatibles avec le modèle VGG16.

2. Utilisation de la Bibliothèque Keras
Le projet implique l'utilisation de la bibliothèque Keras, qui est une API de haut niveau pour le développement de réseaux de neurones. Vous devrez vous familiariser avec les fonctionnalités de Keras pour construire et entraîner votre modèle.

3. Chargement d'un Modèle CNN depuis Keras
Vous utiliserez un modèle pré-entraîné de Convolutional Neural Network (CNN) appelé VGG16, disponible dans Keras. Vous devrez charger ce modèle et le configurer pour votre application spécifique.

4. Application du Transfer Learning
L'une des principales tâches du projet est d'appliquer la technique du Transfer Learning sur le modèle VGG16. Cela signifie que vous allez réutiliser les couches pré-entraînées du modèle VGG16 et les adapter pour résoudre le problème de détection de masque.

5. Tests à partir de la Webcam
Une fois le modèle formé, vous devez développer un système capable de capturer des images depuis la webcam d'un ordinateur en temps réel et d'utiliser le modèle pour déterminer si la personne devant la webcam porte un masque ou non.

Les étapes du projet
Partie 1 : Base de données, Analyse et Préparation
Téléchargez la base de données d'images à partir du lien fourni.
Chargez les images et assurez-vous de les redimensionner selon les exigences du modèle VGG16.
Effectuez la préparation des données nécessaire pour adapter les images au modèle VGG16.
Divisez les données en ensembles d'apprentissage, de validation et de test.
Visualisez des exemples d'images des classes "Avec_Masque" et "Sans_Masque".
Partie 2 : Architecture CNN sur Keras
Appliquez la Data Augmentation sur les données d'apprentissage pour augmenter la variabilité des données.
Chargez et configurez le modèle VGG16 pour votre application.
Utilisez le ModelCheckpoint pour sauvegarder le meilleur modèle pendant l'apprentissage.
Démarrez l'apprentissage en utilisant les données d'apprentissage et de validation, en enregistrant l'historique de l'apprentissage.
Tracez les courbes d'accuracy et d'erreur pour l'ensemble d'apprentissage et de validation.
Calculez l'accuracy et créez la matrice de confusion pour les données de test.
Partie 3 : Application
Testez le modèle développé sur de nouvelles images, que vous pouvez trouver sur Internet ou capturer vous-même.
Affichez le résultat du modèle en indiquant "Avec masque" ou "Sans masque" sur l'image à l'aide de la bibliothèque OpenCV (cv2.putText()).
Développez un code Python qui active la webcam de l'ordinateur et utilise le modèle pour identifier si la personne devant la webcam porte un masque ou non, en affichant un message en temps réel.
Ce projet combine des compétences en manipulation d'images, en apprentissage supervisé avec des réseaux de neurones convolutionnels, et en traitement d'images en temps réel. Il permettra de créer un outil de détection de port de masque utile dans divers contextes.
