# 📅 Calendrier Puzzle Solver

## 📌 Description

Ce projet est un **solveur de puzzle calendrier** développé en langage C.

Le but est de placer **10 pièces différentes sur une grille 8x8** afin de compléter un calendrier selon une date donnée :

- jour
- mois
- jour de la semaine

Le programme utilise :
- le **backtracking**
- les **bitmasks (optimisation mémoire)**
- le **multithreading (pthread)** pour accélérer la recherche

---

## 🚀 Objectif

Trouver **toutes les solutions possibles** pour une date donnée en optimisant les performances du solveur.

---

## 📁 Structure du projet

```text
.
├── main.c
├── solver.c
├── global.c
├── calendrier_puzzle_projet.h
├── Makefile
└── README.md
```

### 📄 Description des fichiers

- **main.c** → interface utilisateur et lancement du programme  
- **solver.c** → algorithme de résolution (backtracking + threads)  
- **global.c** → données globales et gestion du calendrier  
- **calendrier_puzzle_projet.h** → structures et constantes du projet  
- **Makefile** → compilation automatique  

---

## ⚙️ Fonctionnement

1. L’utilisateur entre une date :
```text
jour mois weekday
```

2. Le programme :
- initialise la grille
- génère les pièces et leurs configurations
- lance le solveur multi-threadé
- explore toutes les possibilités

3. Résultat affiché :
- nombre de solutions
- temps d’exécution

---

## 📊 Résultats

Exemple d’exécution :

- 🔢 Nombre de solutions : **1518**
- ⏱️ Temps d’exécution : **7.170 secondes**

⚠️ Les performances peuvent varier selon :
- le processeur
- le nombre de threads
- la date choisie

---

## ▶️ Compilation

```bash
make
```

---

## ▶️ Exécution

```bash
./puzzle
```

---

## 🧠 Concepts utilisés

- Backtracking
- Bitmasks (uint64_t)
- Multithreading (pthread)
- Optimisation algorithmique
- Recherche exhaustive

---

## 🎯 Objectif pédagogique

Ce projet permet de comprendre :

- la résolution de problèmes complexes
- l’optimisation des algorithmes
- la programmation multi-threadée en C
- la gestion mémoire efficace

