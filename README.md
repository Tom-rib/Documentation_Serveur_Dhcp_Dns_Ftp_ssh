# Installation et configuration d'un serveur DHCP, DNS, SSH et FTP sur Debian

Ce projet a pour objectif d'installer et de configurer un serveur DHCP, DNS, SSH et FTP sur deux machines virtuelles Debian sans interface graphique.

---

## Table des matières

1. [Prérequis](#1-prérequis)
2. [Étapes](#2-étapes)
   - [Installation de Debian sans interface graphique](#21-installation-de-debian-sans-interface-graphique)
   - [Mise à jour des systèmes](#22-mise-à-jour-des-systèmes)
   - [Configuration du Serveur DHCP](#23-configuration-du-serveur-dhcp)
   - [Installation du Serveur FTP et SSH](#24-installation-du-serveur-ftp-et-ssh)
   - [Installation du Serveur DNS](#25-installation-du-serveur-dns)
   - [Test de Connexion au Serveur SFTP](#26-test-de-connexion-au-serveur-sftp)

---

## 1. Prérequis

- Deux machines virtuelles Debian sans interface graphique.
- Un réseau virtuel créé par le logiciel de virtualisation.

---

## 2. Étapes

### 2.1 Installation de Debian sans interface graphique

Mettez en place deux machines virtuelles Debian sans interface graphique dans un réseau virtuel créé par votre logiciel de virtualisation.

---

### 2.2 Mise à jour des systèmes

Vérifiez et appliquez les mises à jour nécessaires sur les deux machines Debian afin de garantir un environnement sécurisé et fonctionnel.

---

### 2.3 Configuration du Serveur DHCP

- Installez un serveur DHCP sur la première machine.
- Configurez le serveur DHCP pour attribuer des adresses IP de classe B aux machines connectées au réseau.
- Assurez-vous que la machine hébergeant le serveur DHCP possède une adresse IP fixe.

---

### 2.4 Installation du Serveur FTP et SSH

- Sur la deuxième machine, installez un serveur FTP (proFTP ou vsftpd) ainsi qu'un serveur SSH.
- Configurez le serveur FTP pour permettre l'accès aux utilisateurs (création des répertoires nécessaires et configuration des permissions).
- Configurez le serveur SSH de manière sécurisée, en désactivant les authentifications par mot de passe et en utilisant des clés SSH.

---

### 2.5 Installation du Serveur DNS

- Installez un serveur DNS sur la première machine.
- Configurez le DNS pour que le lien "dns.ftp.com" pointe vers l'adresse IP de la deuxième machine où le serveur FTP est installé.

---

### 2.6 Test de Connexion au Serveur SFTP

- Effectuez les tests de connexion SSH et SFTP depuis une machine cliente.
- Vérifiez que le serveur FTP répond correctement aux requêtes et que le DNS résout le lien "dns.ftp.com".

---
