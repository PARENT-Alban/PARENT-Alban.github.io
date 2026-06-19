---
layout: page
title: "TP R201"
---

# TP R201 : Analyse de flux de l'Internet avec Wireshark et mise en place des paramètres d'un routeur

## 🎯 Objectifs du TP
Analyser concrètement les échanges de trames sur un réseau local pour comprendre le fonctionnement des protocoles essentiels d'Internet (IP, TCP, UDP, ICMP, DNS).

## 🛠️ Technologies et outils utilisés
* Analyseur de protocoles **Wireshark**
* Commandes réseau (ping, traceroute, nslookup)

## 🚀 Notre approche pour le réaliser
Nous avons capturé le trafic réseau pendant des requêtes spécifiques, puis appliqué des filtres d'affichage stricts sur Wireshark pour isoler les flux et analyser la structure des en-têtes.

## 📈 Enseignements, difficultés et ressenti
* **Difficulté :** La quantité massive de paquets capturés simultanément rendait la lecture complexe au début.
* **Enseignement :** Apprentissage de la puissance des filtres Wireshark (ex: `tcp.flags.syn == 1`).
* **Ressenti :** Ce TP m'a permis de "voir" concrètent ce qui circule sur un câble réseau.
