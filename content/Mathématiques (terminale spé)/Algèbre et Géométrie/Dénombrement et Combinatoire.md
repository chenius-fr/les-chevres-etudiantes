---
title: Dénombrement et Combinatoire
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - dénombrement
  - combinatoire
  - probabilités
---

**Thème** : [[Algèbre et Géométrie]]


---

## I - Ensembles et cardinaux

> **Définitions de base**
> Le **cardinal** d'un ensemble fini $E$, noté $\text{Card}(E)$, est le nombre d'éléments qu'il contient.
> Le produit cartésien $E \times F$ est l'ensemble de tous les couples $(x,y)$ avec $x \in E$ et $y \in F$.

**Propriétés fondamentales :**
* **Réunion (formule du crible) :** Pour deux ensembles $A$ et $B$ (pas forcément disjoints) :
  $$\text{Card}(A \cup B) = \text{Card}(A) + \text{Card}(B) - \text{Card}(A \cap B)$$
* **Produit :** $\text{Card}(E \times F) = \text{Card}(E) \times \text{Card}(F)$

---

## II - Les k-uplets (L'ordre compte, répétitions autorisées)

Un $k$-uplet d'un ensemble $E$ à $n$ éléments est une liste ordonnée de $k$ éléments de $E$, qui peuvent se répéter.
*(Exemple type : un code de cadenas, un numéro de téléphone).*

> **Théorème des k-uplets**
> Le nombre de $k$-uplets d'un ensemble à $n$ éléments est égal à :
> $$n^k$$

---

## III - Permutations et Arrangements (L'ordre compte, SANS répétition)

### 1. Les Permutations (Ordonner TOUS les éléments)
Une permutation d'un ensemble $E$ à $n$ éléments est une façon d'aligner la totalité de ces $n$ éléments.
*(Exemple type : le nombre d'anagrammes du mot MATHS, placer des invités autour d'une table).*

> **Théorème des permutations (La factorielle)**
> Le nombre de permutations d'un ensemble à $n$ éléments est noté $n!$ (lire "factorielle n") :
> $$n! = n \times (n-1) \times (n-2) \times \dots \times 2 \times 1$$
> *Par convention, $0! = 1$.*

### 2. Les k-Arrangements (Ordonner UNE PARTIE des éléments)
Un $k$-arrangement est une liste ordonnée de $k$ éléments **distincts** choisis parmi $n$. On pioche sans remettre.
*(Exemple type : l'élection d'un bureau avec Président, Trésorier, Secrétaire).*

> **Théorème des k-arrangements**
> Le nombre de $k$-arrangements parmi $n$ est noté $A_n^k$ :
> $$A_n^k = \frac{n!}{(n-k)!} = n \times (n-1) \times \dots \times (n-k+1)$$

---

## IV - Les Combinaisons (L'ordre NE COMPTE PAS, SANS répétition)

Une combinaison est simplement un sous-ensemble (une poignée) de $k$ éléments piochés simultanément parmi $n$. Puisqu'on les prend d'un coup dans la main, l'ordre d'apparition n'a aucun sens.
*(Exemple type : tirage du Loto, tirer 3 cartes dans un paquet, choisir un comité de 3 élèves).*

> **Théorème des combinaisons (Coefficients binomiaux)**
> Le nombre de combinaisons de $k$ éléments parmi $n$ est noté $\binom{n}{k}$ (lire "k parmi n") :
> $$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

---

## V - Propriétés des coefficients binomiaux et Triangle de Pascal

Les combinaisons possèdent des propriétés remarquables très utiles pour simplifier les calculs sans calculatrice :

**Propriétés immédiates :**
* $\binom{n}{0} = 1$ (Il n'y a qu'une façon de ne rien choisir)
* $\binom{n}{n} = 1$ (Il n'y a qu'une façon de tout prendre)
* $\binom{n}{1} = n$ (Il y a $n$ façons de choisir 1 seul élément)

**Symétrie :**
Choisir $k$ éléments, c'est exactement la même chose que d'en rejeter $(n-k)$. Donc :
$$\binom{n}{k} = \binom{n}{n-k}$$

**Formule (ou relation) de Pascal :**
Cette formule permet de construire le célèbre "Triangle de Pascal" en additionnant deux cases consécutives d'une ligne pour trouver la case située en dessous :
$$\binom{n}{k} = \binom{n-1}{k-1} + \binom{n-1}{k}$$