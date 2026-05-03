---
title: Probabilités, variables aléatoires et Loi Binomiale
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - probabilités
  - loi_binomiale
  - arbres
---

**Thème** : [[Probabilités]]

---

## I - Probabilités conditionnelles et Indépendance

### 1. Probabilité conditionnelle
Soient $A$ et $B$ deux événements (avec $p(B) \neq 0$). 
La probabilité de l'événement $A$ sachant que $B$ est réalisé (notée $p_B(A)$) est définie par :
$$p_B(A) = \frac{p(A \cap B)}{p(B)}$$
*Remarque utile pour les arbres : $p(A \cap B) = p(B) \times p_B(A)$.*

### 2. Indépendance
> **Définition de l'indépendance**
> Deux événements $A$ et $B$ sont dits **indépendants** si et seulement si :
> $$p(A \cap B) = p(A) \times p(B)$$
*(Ce qui revient à dire que $p_B(A) = p(A)$, c'est-à-dire que la réalisation de $B$ n'influence pas $A$).*

### 3. Formule des Probabilités Totales
Cette formule sert à calculer la probabilité globale d'un événement situé à l'extrémité d'un arbre pondéré.

> **Théorème (Probabilités Totales)**
> Si les événements $A_1, A_2, \dots, A_n$ forment une partition de l'univers (ils sont disjoints et leur réunion forme tout l'univers), alors pour tout événement $E$ :
> $$p(E) = p(E \cap A_1) + p(E \cap A_2) + \dots + p(E \cap A_n)$$
> Soit, en utilisant les probabilités conditionnelles :
> $$p(E) = p(A_1) \times p_{A_1}(E) + p(A_2) \times p_{A_2}(E) + \dots$$

---

## II - Variables Aléatoires

Une variable aléatoire $X$ est une fonction qui associe un nombre réel à chaque issue d'une expérience aléatoire (ex: le gain en euros à un jeu).

### 1. Loi de probabilité
Donner la loi de probabilité de $X$, c'est lister dans un tableau toutes les valeurs possibles $x_i$ prises par $X$, et y associer leur probabilité $p_i = p(X = x_i)$.
*Rappel : La somme de toutes les probabilités $p_i$ vaut toujours 1.*

### 2. Espérance, Variance et Écart-type
* **L'Espérance $E(X)$** (la moyenne que l'on peut espérer obtenir si on répète l'expérience un très grand nombre de fois) :
  $$E(X) = p_1 x_1 + p_2 x_2 + \dots + p_n x_n = \sum_{i=1}^{n} p_i x_i$$
* **La Variance $V(X)$** et **l'Écart-type $\sigma(X)$** (mesurent la dispersion des valeurs autour de l'espérance) :
  $$V(X) = \sum_{i=1}^{n} p_i (x_i - E(X))^2$$
  $$\sigma(X) = \sqrt{V(X)}$$

> **Propriétés de linéarité (très utiles pour les changements d'unités ou de mise de départ) :**
> Pour tous réels $a$ et $b$ :
> * $E(aX + b) = a \cdot E(X) + b$
> * $V(aX + b) = a^2 \cdot V(X)$
> * $\sigma(aX + b) = |a| \cdot \sigma(X)$

---

## III - Le Schéma de Bernoulli et la Loi Binomiale

C'est le modèle probabiliste le plus important du lycée. Il modélise les situations de type "Succès/Échec" répétées plusieurs fois.

### 1. Épreuve et Schéma de Bernoulli
* **Épreuve de Bernoulli :** Expérience aléatoire ne comportant que deux issues : un "Succès" (de probabilité $p$) et un "Échec" (de probabilité $1-p$).
* **Schéma de Bernoulli :** Répétition de $n$ épreuves de Bernoulli, de manière **identique et indépendante**.

### 2. La Loi Binomiale $\mathcal{B}(n, p)$
Soit $X$ la variable aléatoire comptant le **nombre de succès** obtenus lors d'un schéma de Bernoulli de paramètres $n$ (nombre d'essais) et $p$ (probabilité du succès).
On dit que $X$ suit la loi binomiale $\mathcal{B}(n, p)$.

> **Formule de la probabilité**
> Pour tout entier $k$ (compris entre $0$ et $n$), la probabilité d'obtenir exactement $k$ succès est :
> $$p(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$$
*(Rappel : $\binom{n}{k}$ est le coefficient binomial qui compte le nombre de chemins menant à $k$ succès sur l'arbre).*

> **Espérance et Variance de la loi Binomiale**
> Ces formules évitent de longs calculs fastidieux :
> * $E(X) = n \times p$
> * $V(X) = n \times p \times (1-p)$