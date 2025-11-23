# Optimisation de la Fonction de Himmelblau avec SymPy

## Description

Ce projet utilise **SymPy** pour explorer l'optimisation de la **fonction de Himmelblau** à l'aide de la méthode de **descente de gradient**. La fonction de Himmelblau est une fonction test classique en optimisation numérique, connue pour ses **quatre minima locaux** égaux à zéro.

La fonction est définie par :
\[ f(x, y) = (x^2 + y - 11)^2 + (x + y^2 - 7)^2 \]

## Caractéristiques de la Fonction

- **4 minima locaux** avec \( f(x, y) = 0 \) :
  - \( (3, 2) \)
  - \( (-2.805, 3.131) \)
  - \( (-3.779, -3.283) \)
  - \( (3.584, -1.848) \)
- **Point de départ** : \( (7, 1.5) \)
- **Points critiques** : Solutions du système d'équations \(\nabla f(x, y) = 0\).
- **Surface complexe** avec plusieurs bassins d'attraction.

## Gradient de la Fonction

Le gradient de la fonction de Himmelblau est donné par :
\[ \nabla f(x, y) = \begin{pmatrix}
4x(x^2 + y - 11) + 2(x + y^2 - 7) \\
2(x^2 + y - 11) + 4y(x + y^2 - 7)
\end{pmatrix} \]

## Méthode d'Optimisation

### Descente de Gradient

La descente de gradient est une méthode itérative pour trouver les minima d'une fonction. Elle est définie par :
\[ \mathbf{x}_{k+1} = \mathbf{x}_k - \alpha \nabla f(\mathbf{x}_k) \]
où \(\alpha\) est le **pas d'apprentissage**.

### Choix du Pas

#### Pas Optimal

Le **pas optimal** est calculé pour minimiser la fonction à chaque itération. Cependant, ce calcul est **coûteux en temps** et nécessite des ressources computationnelles importantes.

#### Pas Fixe

Pour contourner ce problème, nous utilisons des **pas fixes** pour la descente de gradient. Les valeurs de pas testées sont :
- 0.325
- 0.25
- 0.125
- 0.05
- 0.01

Ces valeurs permettent de trouver un compromis entre la **rapidité de convergence** et la **stabilité de l'algorithme**.

## Résultats

### Tableau Comparatif

| Méthode      | Pas α   |
|--------------|---------|
| Optimal      | Optimal | 
| Fixe         | 0.325   | 
| Fixe         | 0.25    | 
| Fixe         | 0.125   | 
| Fixe         | 0.05    | 
| Fixe         | 0.01    | 
### Observations

- **Pas optimal** : Bien que plus précis, le calcul du pas optimal est **trop coûteux** pour être utilisé dans ce contexte.
- **Pas fixes** : Les pas fixes permettent une **convergence rapide** et **stable** vers les minima locaux, avec un coût computationnel bien inférieur.
- **Pas de 0.05** : Offre un bon compromis entre rapidité de convergence et précision.

## Visualisation

Les résultats sont visualisés à travers plusieurs graphiques :
- **Trajectoires de descente** : Comparaison des chemins empruntés par les différentes méthodes.
- **Évolution de la fonction objectif** : Montre comment la valeur de la fonction diminue au fil des itérations.
- **Norme du gradient** : Évolution de la norme du gradient, indiquant la convergence vers un minimum.
- **Points finaux** : Localisation des points finaux atteints par chaque méthode.

## Conclusion

L'utilisation de **pas fixes** pour la descente de gradient sur la fonction de Himmelblau s'est avérée efficace. Malgré la précision théorique du pas optimal, son coût computationnel élevé rend les pas fixes plus pratiques pour des applications réelles.

## Comment Exécuter le Code

1. **Prérequis** :
   - Python 3.x
   - Bibliothèques : `numpy`, `sympy`, `matplotlib`

2. **Installation** :
   ```bash
   pip install numpy sympy matplotlib

## Auteur : 
TAGNE TALLA IDRISS CHANEL
DJATCHE KAMGAIN SYLVANO
ESSUTHI MBANGUE ANGE ARMEL
GOUJOU GUIMATSA

