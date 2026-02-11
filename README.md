# Mini-Projet IoT – Maison Connectée

# Description

Ce mini-projet consiste à installer, configurer et contrôler des périphériques IoT dans un environnement de maison connectée en utilisant Cisco Packet Tracer 7.0 ou version ultérieure. Les périphériques IoT sont connectés au réseau domestique via une passerelle domestique (Home Gateway) et peuvent être contrôlés localement ou à distance via un serveur d'enregistrement.

# Objectifs

-Configurer un réseau domestique sans fil pour connecter des périphériques IoT.

-Enregistrer les périphériques IoT auprès d’un serveur distant.

-Contrôler les périphériques IoT localement ou via une interface Web.

-Vérifier la connectivité entre les équipements de la maison et le serveur distant.

# Matériel et Logiciels

Logiciel : Cisco Packet Tracer 7.0 ou version ultérieure

Périphériques : Lampe, ventilateur de plafond, humidificateur, pot de café

Ordinateur à carte unique (SBC) simulé dans Packet Tracer

Home Gateway et modem simulés

Serveur IoT distant : www.register.pka

Compte serveur :

Nom d’utilisateur : admin

Mot de passe : admin



# Instructions

- Partie 1 : Configuration de la maison connectée

/Configurer le réseau sans fil

Home Gateway → Config → Internet → DHCP activé.

Home Gateway → Wireless → SSID : MyHomeGateway → WPA2-PSK → clé : CiscoIoT.

PC sans fil → Connexion au réseau MyHomeGateway avec la clé CiscoIoT.

/Connecter les périphériques IoT

Pour chaque périphérique (Lampe, ventilateur, humidificateur, pot de café) :

Config → Wireless0 → SSID : MyHomeGateway

WPA2-PSK → clé : CiscoIoT

IP : DHC



- Partie 2 : Configuration du réseau distant

/Connecter le Home Gateway au modem via un câble.

/Configurer les interfaces :


Home Gateway : LAN 192.168.25.1/24 et Internet 200.10.10.9/24

Serveur IoT : FastEthernet 200.10.10.10/24, Cellulaire 3G/4G 201.10.10.11/24

Activer IoT Service et DNS sur le serveur.

/Vérifier la connectivité entre le Laptop domestique et le serveur.


- Partie 3 : Interagir avec les périphériques IoT

/Accès local

Alt + clic sur chaque périphérique pour tester le contrôle direct.

/Accès distant via serveur d’enregistrement

Pour chaque périphérique → Config → Serveur distant → Adresse : www.register.pka ou 200.10.10.10

Nom d’utilisateur : admin, Mot de passe : admin → Se connecter

/Contrôle via interface Web

Laptop → Bureau → Navigateur → www.register.pka

/Connexion avec les identifiants admin/admin

Vérifier et contrôler les périphériques IoT à distance (ex : modifier l’intensité de la lampe)


# Résultat attendu

Les périphériques IoT sont connectés et fonctionnent correctement sur le réseau domestique.

L’accès local et distant via serveur d’enregistrement est opérationnel.

Les changements effectués via l’interface Web se répercutent sur les périphériques.

# Auteur
Ranim Mili 
