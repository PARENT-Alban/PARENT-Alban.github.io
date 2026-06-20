---
layout: page
title: "SAÉ 22"
---

# SAÉ 22 : Synthèse sonore et simulation d'effets guitare sous MATLAB

## 🎯 Objectif du projet
L'objectif de cette SAÉ était de se familiariser avec le traitement de base des signaux (synthèse et filtrage) en utilisant des signaux sonores. Le but était d'implanter l'algorithme de modèle de corde pincée de Karplus-Strong pour générer artificiellement des notes de guitare réalistes, puis de coder une pédale d'effet audio pour personnaliser le rendu d'une partition numérique de 10 secondes.

## 🛠️ Technologies et outils utilisés
* Environnement de programmation algorithmique : **MATLAB**
* Algorithme central : **Modèle Karplus-Strong** (excitation par *noise burst* de bruit blanc, ligne à retard $DL_k$ calculée selon la fréquence d'échantillonnage $F_e = 44100$ Hz et la note $F_0$).
* Traitement du signal : Filtre passe-bas d'ordre 1 (moyenne d'échantillons), analyse fréquentielle par transformée de Fourier rapide (`fft`), et fonctions de rendu audio (`soundsc`).
* Effets implémentés : Conception algorithmique d'effets guitare (saturation/distorsion ou modulation de signal).

## 🚀 Les défis rencontrés & Solutions
* **Défi :** Réussir à implémenter correctement la ligne à retard et le bouclage du filtre passe-bas dans la boucle temporelle `for...end` sans créer de décalage de hauteur ou de distorsion numérique involontaire.
* **Solution :** Suivi rigoureux des équations de propagation du signal ($DL_k(1) = s(k)$ après décalage) et ajustement du gain d'atténuation $a$ entre 0.97 et 0.99 pour contrôler précisément le temps de chute (l'écrasement naturel) de la note après l'attaque.

## 📈 Résultats obtenus et compétences acquises
* Génération réussie de notes pures aux fréquences harmoniques parfaites, exécution d'une partition complète de 10 secondes et application d'une pédale d'effet audio logicielle fonctionnelle.
* **Compétence validée :** *Compétence 2 — Connecter les entreprises et les usagers (Compréhension de la couche physique et du traitement numérique du signal)*. J'ai appris à lier les concepts abstraits des mathématiques du signal (spectres, fréquences de coupure, filtres) à des applications concrètes de programmation et de traitement de données acoustiques.
