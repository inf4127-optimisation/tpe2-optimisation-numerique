# 📉 TPE : Algorithmes d'Optimisation Numérique Sans Contraintes

**Université de Yaoundé I** **Département d'Informatique** **Cours :** INF4127 - Optimisation 2  
**Enseignant :** Pr. MELATAGIA  
**Année Académique :** 2024-2025

---

## 👥 Membres du Groupe
| Matricule | Nom & Prénom | Rôle / Fonction Traitée |
|-----------|--------------|-------------------------|
| **24F2456** | **ESSUTHI MBANGUE Ange Armel** | **Rosenbrock & Architecture GitHub** |
| **19M2351**| **TAGNE TALLA Idriss** | **Fonction de Himmelblau(Point Selle)** |
| **22W2163** | **DJATCHE-NKAMGANG Sylvano** | **Fonction Quadratique** |
| **21T2899** | **GOUJOU GUIMATSA Zidane** | **Analyse et Rapports** |

---

## 📝 Description du Projet

Ce dépôt contient les travaux pratiques encadrés (TPE) portant sur l'implémentation et l'analyse des **méthodes de descente de gradient** pour l'optimisation numérique sans contraintes.

L'objectif est de minimiser des fonctions $f: \mathbb{R}^n \to \mathbb{R}$ en comparant deux approches :
1.  **Méthode à Pas Fixe :** $x_{k+1} = x_k - \alpha \nabla f(x_k)$
2.  **Méthode de la Plus Profonde Descente (Steepest Descent) :** Le pas $\alpha_k$ est optimisé à chaque itération via une recherche linéaire (Line Search).

Le projet inclut des **visualisations dynamiques** (animations vidéo) pour illustrer la convergence des algorithmes.

---

## 🧪 Fonctions Étudiées

Nous avons analysé le comportement des algorithmes sur trois fonctions aux topologies caractéristiques :

### 1. La Fonction de Rosenbrock ("Vallée de la Banane")
$$f(x, y) = (1 - x)^2 + 100(y - x^2)^2$$
* **Minimum Global :** $(1, 1)$ où $f=0$.
* **Difficulté :** Le minimum se trouve dans une vallée étroite, courbe et plate.
* **Observation :** La méthode à pas fixe est lente mais stable. La méthode à pas optimal génère des zig-zags (directions orthogonales) très inefficaces dans la vallée.

### 2. La Fonction Quadratique (Point Selle)
$$f(x, y) = x^2 - y^2$$
* **Point Critique :** $(0, 0)$ ($\nabla f = 0$).
* **Difficulté :** Ce n'est ni un minimum ni un maximum. La fonction est convexe en $x$ et concave en $y$.
* **Observation :** L'algorithme diverge vers $-\infty$ le long de l'axe $y$. Cela illustre le danger des points selles et l'importance de la convexité.

### 3. La Fonction de Himmelblau (ou autre fonction traitée)
*(À compléter selon ce que tes amis ont fait, généralement c'est celle-ci :)*
$$f(x, y) = (x^2 + y - 11)^2 + (x + y^2 - 7)^2$$
* **Particularité :** Possède 4 minimums globaux identiques.
* **Observation :** Le point de convergence dépend uniquement du point de départ choisi (Bassin d'attraction).

---

## 📂 Structure du Dépôt

```bash
TP-OPtimisation-Descente_De_Gradient/
├── notebooks/                  # Codes sources Jupyter
│   ├── Rosenbrock.ipynb        # Analyse complète Rosenbrock (avec Vidéos)
│   ├── Quadratique.ipynb       # Analyse Point Selle
│   └── Himmelblau.ipynb        # Analyse Multi-modale
├── doc/                        # Cahiers de suivi individuels
│   ├── 24F2456AngeArmelESSUTHI.md
│   ├── MatriculeNomPrenom.md
│   └── ...
├── images/                     # Captures d'écran et graphiques générés
├── README.md
MIT Licence     #Fichier
        