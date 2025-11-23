# Cahier de Suivi - ESSUTHI MBANGUE ANGE ARMEL
**Matricule:** 24F2456  
**Projet:** TPE Optimisation Numérique & Calcul Symbolique  
**Cours:** INF4127 - Optimisation 2  
**Encadreur:** Pr. MELATAGIA  

---

## Séance 1 - 1 Octobre 2025
### Activités réalisées :
- [x] Création du notebook Jupyter complet avec SymPy
- [x] Implémentation des 10 blocs de calcul symbolique
- [x] Développement des fonctions de manipulation algébrique
- [x] Implémentation du calcul différentiel et des gradients
- [x] Création des visualisations avec Matplotlib

### Difficultés rencontrées :
- Compréhension des différences symbolique/numérique
- Gestion des erreurs de substitution dans les matrices
- Conversion symbolique → numérique avec lambdify

### Solutions apportées :
- Tests pratiques bloc par bloc
- Debuggage des fonctions de substitution
- Utilisation de dictionnaires pour les substitutions

### Temps passé : 6 heures

---

## Séance 2 - 2 Octobre 2025
### Activités réalisées :
- [x] Finalisation des applications en optimisation
- [x] Résolution des problèmes de classification des points critiques
- [x] Création de la structure GitHub et documentation
- [x] Rédaction des fichiers README et suivi individuel
- [x] Préparation de la présentation finale

### Difficultés rencontrées :
- Résolution des erreurs avec les matrices Hessiennes
- Organisation de la structure des dossiers selon les consignes
- Gestion des formats de retour de SymPy

### Solutions apportées :
- Correction étape par étape avec assistance IA
- Création de la structure doc/ exigée
- Adaptation du code pour gérer différents formats

### Temps passé : 5 heures

---

## Séance 3 - 22 Octobre 2025 (Présentation de Groupe)
**Sujet :** Toolbox d’optimisation non-lisse (UNLocBoX)  
**Membres du groupe :** Essuthi Mbangue, Tagne Talla, Djatche-Nkamgang, Goujou Guimatsa.

### Activités réalisées :
- [x] Conception et rédaction de la présentation sur UNLocBoX (MATLAB/Octave)
- [x] Étude du contexte mathématique : Méthodes proximales et opérateurs proximaux (Prox)
- [x] Analyse de la structure de la toolbox (Solveurs, Démos, Utilitaires)
- [x] Implémentation d'un cas pratique : Reconstruction d'image avec régularisation TV (Total Variation)
- [x] Comparaison des solveurs (FISTA, Douglas-Rachford, Forward-Backward)

### Difficultés rencontrées :
- Compréhension mathématique de l'opérateur proximal pour les fonctions non-différentiables ($\ell_1$, TV)
- Configuration de l'environnement MATLAB/GNU Octave pour les dépendances
- Formulation du problème inverse $y = Ax + n$ sous forme de splitting proximal

### Solutions apportées :
- Décomposition du problème en sommes de fonctions convexes ($f_1$ différentiable + $f_2$ non-lisse)
- Utilisation de la fonction `solvep` pour la sélection automatique du solveur
- Rédaction d'une documentation claire sur l'installation et les limitations

### Temps passé : 5 heures

---

## Séance 4 - 23 Novembre 2025
### Activités réalisées :
- [x] Étude approfondie de la fonction de Rosenbrock ("Vallée de la Banane")
- [x] Implémentation de l'algorithme de Descente de Gradient à Pas Fixe
- [x] Implémentation de la méthode du Pas Optimal (Steepest Descent) avec `scipy`
- [x] Génération d'animations vidéo pour visualiser la convergence en temps réel
- [x] Analyse comparative : Stabilité (Pas fixe) vs Phénomène de "Zig-Zag" (Pas optimal)

### Difficultés rencontrées :
- Calcul correct des dérivées partielles (Gradient) pour Rosenbrock
- Compréhension théorique de pourquoi le "Pas Optimal" génère des trajectoires orthogonales inefficaces
- Visualisation dynamique (animation) de l'algorithme dans le Notebook

### Solutions apportées :
- Vérification mathématique du gradient étape par étape
- Création de DataFrames Pandas pour suivre l'évolution précise de la norme du gradient
- Rédaction d'une analyse interprétative liant la topologie de la vallée au comportement de l'algorithme

### Temps passé : 4 heures

---

## Bilan Final
**Temps total investi :** 20 heures  
**Pourcentage de contribution :** 100% (Impliqué dans toutes les phases)  
**Statut :** Projet terminé et entièrement documenté

## Compétences acquises et Fonctions développées :
- **Calcul Symbolique :** Maîtrise de SymPy pour le calcul exact et l'algèbre linéaire.
- **Optimisation Convexe Non-Lisse :** Compréhension des opérateurs proximaux et utilisation de UNLocBoX.
- **Optimisation Numérique :** Implémentation et analyse critique des algorithmes de descente (Gradient, Steepest Descent).
- **Visualisation Scientifique :** Création de graphiques 3D, lignes de niveau et animations de convergence.
- **Travail d'équipe :** Coordination pour la présentation de groupe et rédaction technique.