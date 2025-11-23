# 🎓 Projet: Optimisation de la Fonction de Rosenbrock f(x,y) = (1-x)² + 100(y-x²)²

**Cours:** INF4127 - Optimisation 2  
**Institution:** Université de Yaoundé 1  
**Année Académique:** 2024-2025  
**Encadreur:** Pr. MELATAGIA YONTA PAULIN

---

## 👥 Équipe du Projet

| Matricule | Nom | Prénom |
|-----------|-----|--------|
| 22W2163 | DJATCHE-NKAMGANG | SYLVANO |
| 24F2456 | ESSUTHI MBANGUE | ANGE ARMEL |
| 19M2351 | TAGNE TALLA | IDRISS CHANEL |
| 21T2899 | GOUJOU GUIMATSA | ZIDANE |

---

## 📋 Table des Matières

1. [Introduction](#introduction)
2. [Description de la Fonction](#description-de-la-fonction)
3. [Méthodologie](#méthodologie)
4. [Implémentation](#implémentation)

---

## 📖 Introduction

Ce projet porte sur l'optimisation numérique sans contraintes de la fonction de Rosenbrock, une fonction-test classique en optimisation. L'objectif est d'implémenter et de comparer différentes méthodes de descente pour trouver le minimum global de cette fonction.

## 🎯 Description de la Fonction

### Fonction de Rosenbrock
\[ f(x, y) = (1 - x)^2 + 100(y - x^2)^2 \]

**Caractéristiques principales:**
- Minimum global en (1, 1) avec f(1,1) = 0
- Vallée étroite et courbée ("banana valley")
- Conditionnement difficile
- Point critique unique

**Gradient:**
\[ \nabla f(x, y) = \begin{bmatrix} -2(1-x) - 400x(y-x^2) \\ 200(y-x^2) \end{bmatrix} \]

## 🔬 Méthodologie

### 1. Méthode de Gradient à Pas Optimal
- Direction de descente: \( d_k = -\nabla f(x_k) \)
- Pas optimal déterminé par recherche linéaire exacte
- Méthode de la section dorée pour la minimisation unidimensionnelle

### 2. Méthode de Gradient à Pas Fixe
- Direction de descente: \( d_k = -\nabla f(x_k) \)
- Pas constant prédéfini
- Plusieurs valeurs de pas testées pour analyse comparative

### Critères d'arrêt:
- Norme du gradient: \( \|\nabla f(x_k)\| < \varepsilon \)
- Stagnation de la solution
- Nombre maximum d'itérations

## 💻 Implémentation

### Structure du Code
```python
# Fonctions principales
def rosenbrock(x, y)
def grad_rosenbrock(x, y)
def gradient_pas_optimal(f, grad_f, x0, y0, ...)
def gradient_pas_fixe(f, grad_f, x0, y0, pas, ...)

Dépendances

    NumPy pour les calculs numériques

    Matplotlib pour la visualisation

    SymPy pour l'analyse symbolique
   
Observations Clés

    Méthode à Pas Optimal:

        Convergence plus rapide que le pas fixe

        Phénomène de zigzag caractéristique dans la vallée

        Adaptation automatique du pas à la courbure locale

    Méthode à Pas Fixe:

        Sensibilité élevée au choix du pas

        Convergence lente pour des pas trop petits

        Divergence possible pour des pas trop grands

        Comportement plus stable mais moins efficace

