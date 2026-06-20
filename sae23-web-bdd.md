---
layout: page
title: "SAÉ 23"
---

# SAÉ 23 : Mettre en place une solution informatique d'entreprise (Web & BDD)

## 🎯 Objectif du projet
L'objectif de cette SAÉ était de concevoir et de développer une application web dynamique reliée à une base de données relationnelle. Le projet consistait à modéliser une base de données (contenant par exemple des tables pour les courses, les skippers et les bateaux), et à créer une interface permettant d'afficher, de manipuler et de mettre à jour ces données en temps réel.

## 🛠️ Technologies et outils utilisés
* **Back-end :** Servlets écrits en **Java** pour gérer la logique de l'application et assurer la connexion et les requêtes directes vers la base de données.
* **Base de données :** Système de Gestion de Base de Données Relationnelles (SGBD) pour structurer les tables et lier les entités entre elles.
* **Front-end :** Interface utilisateur interactive programmée en HTML5 et **JavaScript** pour gérer l'affichage dynamique et les interactions.

## 🚀 Les défis rencontrés & Solutions
* **Défi :** Réussir à lier correctement les actions de l'utilisateur sur l'interface avec le traitement back-end en Java, notamment lors de la manipulation ou de la transmission des identifiants (`Course`, `Skipper`, `Bateau`) dans les fonctions JavaScript.
* **Solution :** Débogage rigoureux des fonctions de traitement et des servlets Java pour s'assurer que chaque identifiant sélectionné côté client soit correctement intercepté, afin que le serveur puisse interroger la base de données pour récupérer la bonne ligne et renvoyer les informations correspondantes à afficher.

## 📈 Résultats obtenus et compétences acquises
* Déploiement réussi d'une application web dynamique fonctionnelle permettant d'administrer et de visualiser les classements et les informations de la base de données.
* **Compétence validée :** *Compétence 3 — Créer des outils et applications pour les R&T*. J'ai développé une vision concrète de l'interaction entre une interface utilisateur, du script de contrôle et une base de données relationnelle.
