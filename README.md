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



!\[Photo](Montage LM35 et ESP32.jpg)





Nous obtenons le montage ci-dessous :



## PHOTO



Nous avons aussi relié le Raspberry-Pi à l'ordinateur comme ceci :



## PHOTO



### II. Acquisition et transmission des données

L'objectif dans cette partie est d'acquérir les données de température du capteur LM35 et les transmettre sur Node-red via MQTT et la connexion Wi-Fi. Le schéma explicatif se présente comme ci-dessous :



#### CAPTURE SCHEMA

#### 

La première étape est d'acquérir les données de température du capteur LM35. Pour cela, nous exécutons le programme Arduino ci-dessous.



### Capture programme Arduino



Ensuite, on s'occupe du Raspberry-Pi avec la mise en place du MQTT et du Mosquitto. Mosquitto et le broker MQTT ont déjà été installés et configurés lors d'un TD pour interdire les utilisateurs anonymes de se connecter sur le broker (mise en place d'un identifiant et d'un mot de passe déjà crées) et que le broker soit accessible sur le port 1883. On active le broker Mosquitto dans le terminal à l'aide de la commande: "sudo systemctl start mosquitto". Pour rendre le Raspberry autonome avec le broker avec le borker qui tourne dès qu'il est alimenté, on utulise cette commande: "sudo systemctl enable mosquitto". Ensuite, on tente de se connecter au serveur 





##### 

