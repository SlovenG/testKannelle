# testKannelle

Dans l'optique de pouvoir développer une application Android permettant l'édition de Vidéo, les problématiques sont les suivantes :

  1: trouver une librairie native ou non permettant l'édition de video ou la manipulation de celle-ci
  
  2: indentifier les "editing" de vidéo que l'on veut implementer au sein de l'app
  
  3: implementer la partie traitement vidéo en offline: depuis le Device Android
  
  
 
 
 Forcé de constater que l'édition de vidéo sur Android est bien moins evidente et surtout accessible que sur iOS avec sa librairie AVFoundation permettant l'editoring
 de vidéo avec une api claire et facile d'utilisation, il en est bien différent de la partie Android : Aucune librairie native n'a été développé à ce jour, cependant Android laisse la possibilité de pouvoir le faire via des librairies externes et en utilisant
 le NDK Android (Native Development Kit) permettant l'écriture de ces librairies dans différents langages autre que le natif(Java/Kotlin).
 L'utilisation du Ndk est d'autant plus complexe que l'on demande d'avoir une très (très) bonne connaissance du SDK Android dans sa totalité.
 
 Quelques librairies externes tels que Magisto permettent l'edition de vidéo simple via une API, mais le soucis etant que toute la partie traitement de video se fait Online coté serveur, celles-ci ne répondant pas à la problematique du processing on Device.
Il reste enfin des librairies universelles tels que FFMPEG certes datant d'une autre époque mais permmettant l'edition de video/image  depuis le Device mais pour la compilé on devra également utilisé le NDK Android.
En plus de son intégration compliqué, il reste a savoir si cette librairie permet l'utilisation d'animation de dernière génération faites par des logiciels tels que Adobe After Effect.

En ayant fait le tour de toutes ces spécifications techniques, il a fallu se mettre a l'évidence que cela n'allait pas être aussi simple. Donc j'ai pris le problème d'un autre angle, regardant les technologies Cross-Platforme gérant les animations dans un soucis d'avoir deux comportements similaires sur Android et iOS dans leur environnement natif respectif.

le choix c'est tourné vers Lottie: libriairie developpé par Airbnb permettant l'intégration d'animation faites sur After Effects les générants via le plug-in ae:bodymovin en Json pouvant alors être intégré quelque soit le support React,Android,iOS de manière fluide et customisable.

Et pour le fait de pouvoir enregistrer ensuite la video comportant les animations, l'idée qui m'est parvenue est le Screen Cast, developpé en natif depuis KitKat (SDK 21) permettant d'enregistrer toutes ou parties de son Device en vidéos de différentes qualités possibles.
Cette partie est la solution par defaut n'ayant pas trouvé de moyen de pouvoir enregistrer les supperpositions d'animations Lottie (After Effects)/videos de manière techniquement correcte pour un vidéaste.

Description du projet:
  Video implementé
  animation lottie integré par desssus la vidéo
  la possibilité de Screen Record le rendu, le chemin de la vidéo étant accessible dans le dossier SDCARD du Device ou Simulateur .
  
N'ayant pas reussi a implementer tout ce que j'aurais voulu, j'ai tout de meme vu que tout ceci etait possible en denichant une App:Kinemaster permettant l'editing de vidéos de facon simple et ergonomique pour un usage sur Smartphone.

Ce projet est voué a être un vrai challenge pour les développeurs travaillant sur celui-ci :)

