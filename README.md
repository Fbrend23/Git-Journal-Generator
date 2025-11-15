# Git Journal Generator

Ce projet fournit un script permettant de générer automatiquement un **journal de travail** en Markdown à partir de l’historique Git d’un projet.  
L’objectif est d’offrir un document clair, structuré par semaine et par jour, idéal pour le suivi scolaire, les rapports de projet ou la documentation d’activité.

Le script produit un fichier `journal.md` contenant :

- un regroupement **par semaine**
- un regroupement **par jour**
- chaque commit avec :
  - la date
  - l’auteur
  - le message
  - un tableau des fichiers modifiés (stat)

Ce journal ne contient que les statistiques de modification, afin de rester lisible et concis.

---

## 📦 Fonctionnalités

- Analyse complète de l’historique Git du projet
- Organisation chronologique (du plus ancien au plus récent)
- Regroupement **par semaine ISO**
- Regroupement **par jour**
- Tableau Markdown pour les fichiers modifiés par commit
- Sortie automatique dans `journal.md`
- Compatible Git Bash, WSL et Linux

## ▶️ Utilisation

### 1. Cloner le dépôt

```sh
git clone https://github.com/Fbrend23/Journal-de-travail.git
```

2. Mettre le script à la racine du projet git

3. Lancer la génération du journal avec git bash

```bash
 /journal.sh
```

Un fichier journal.md sera créé à la racine du projet.

# 📝 Exemple de sortie

## Semaine 45 (2025-11-03 → 2025-11-09)

### 2025-11-03

#### Commit a1b2c3d

**Date :** 2025-11-03T14:21:00 — **Auteur :** Brendan Fleurdelys

**Message :** Mise en place du système de sessions

| Fichier   | Modifications            |
| --------- | ------------------------ |
| server.js | 4 insertions             |
| auth.js   | 2 insertions, 1 deletion |

# ⭐ Objectif du projet

Ce script a été conçu pour faciliter la création d’un journal de travail
pour l'ETML.

# 📄 Licence

Libre d’utilisation et de modification.
