# Installation et configuration d'un serveur DHCP, DNS , SSH et FTP  sur Debian

Ce projet a pour objectif d'installer et de configurer un serveur DHCP et un serveur FTP sur deux machines virtuelles Debian sans interface graphique.


##  Table des matières
 
Prérequis

Étapes

Installation de Debian sans interface graphique

Mise à jour des systèmes

Configuration du Serveur DHCP

Installation du Serveur FTP et SSH

Installation du Serveur DNS

Test de Connexion au Serveur SFTP

Paramètres de Sécurité Additionnels

Conclusion


## Prérequis


Deux machines virtuelles Debian sans interface graphique

Un réseau virtuel créé par le logiciel de virtualisation


Étapes

Installation de Debian sans interface graphique


Mettez en place deux machines virtuelles Debian sans interface graphique et dans un réseau virtuel créé par votre logiciel de virtualisation.


Mise à jour des systèmes


Vérifiez et appliquez les mises à jour nécessaires sur les deux machines.


## Configuration du Serveur DHCP


Installez un serveur DHCP sur la première machine.

Configurez le serveur DHCP pour attribuer des adresses de classe B aux machines connectées au réseau.

Assurez-vous que la machine hébergeant le serveur DHCP possède une adresse IP fixe.


## Installation du Serveur FTP et SSH


Sur la deuxième machine, installez un serveur FTP (proFTP ou vsftpd) et un serveur SSH.

Configurez le serveur FTP pour permettre l'accès aux utilisateurs.

Configurez le serveur SSH pour permettre l'accès sécurisé aux utilisateurs.


## Installation du Serveur DNS


Installez un serveur DNS sur la première machine.

Configurez le DNS de sorte que le lien soit "dns.ftp.com", pointant vers l'adresse IP de la deuxième machine où le serveur FTP est installé.


## Test de Connexion au Serveur SFTP
