# testKannelle

Dans l'optique de pouvoir développer une application Android permettant l'édition de Vidéo, les problématiques sont les suivantes :

  1: trouver une librairie native ou non permettant l'édition de video ou la manipulation de celle-ci
  
  2: indentifier les "editing" de vidéo que l'on veut implementer au sein de l'app
  
  3: implementer la partie traitement vidéo en offline: depuis le Device Android
  
  
 
 
 Forcé de constater que l'édition de vidéo sur Android est bien moins evidente et surtout accessible que sur iOS avec sa librairie AVFoundation permettant l'editoring
 de vidéo avec une api claire et facile d'utilisation, il en est bien différent de la partie Android : Aucune librairie native n'a été développé à ce jour, cependant Android laisse la possibilité de pouvoir le faire via des librairies externes et en utilisant
 le NDK Android (Native Development Kit) permettant l'écriture de ces librairies dans différents langages autre que le natif(Java/Kotlin).
 L'utilisation du Ndk est d'autant plus complexe que l'on demande d'avoir une très (très) bonne connaissance du SDK Android dans sa totalité.
 
 Quelques librairies externes tels que Magisto permettent l'edition de vidéo simple via une API, mais le soucis etant que toute la partie traitement de video se fait Online coté serveur, celles-ci ne répondant pas a
