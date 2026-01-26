Akkaya Mikail

Chevrier Séréna

MP3D

#  			Projet suivi température



## Sommaire :

##### Introduction

##### I. Installation du Raspberry-Pi et de l'ESP32

##### II. Acquisition et transmission des données

##### III. Affichage et interface utilisateur

##### IV. Stockage et exploitation des données

##### V. Sécurisation et fiabilité

##### VI. Alertes et Automatisation



## Introduction :

Dans ce projet, nous allons concevoir un système de surveillance de température en utilisant un capteur LM35, une carte ESP32, un Raspberry Pi ainsi que le protocole MQTT. Le but principalement sera de transmettre les données du capteur de température au Raspberry Pi via Mosquitto et le réseau Wi-Fi, les stocker dans une base de données SQLite et les afficher en temps réel à l'aide du Node-Red.



### I. Installation du Raspberry-Pi et de l'ESP32

Tout d'abord, nous avons procédé au montage du capteur de température LM35 et de la carte ESP32 sur une plaque de prototypage, tout en étant vigilants sur les branchements. Les documents ci-dessous montrent comment lier le capteur à la carte :



## CAPTURE



Nous obtenons le montage ci-dessous :



## PHOTO



Nous avons aussi relié le Raspberry-Pi à l'ordinateur comme ceci :



## PHOTO







##### 

