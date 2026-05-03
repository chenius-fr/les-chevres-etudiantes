---
title: Dérivation, composées et convexité
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - dérivation
  - tangente
  - convexité
---

**Thème** : [[Analyse Fonctionnelle]]

---

## I - Rappels : Nombre dérivé et Tangente

### 1. Définition de la dérivabilité
Dire qu'une fonction $f$ est dérivable en un réel $a$ signifie que le taux d'accroissement admet une limite finie quand $h$ tend vers 0 :
$$\lim_{h \to 0} \frac{f(a+h) - f(a)}{h} = f'(a)$$
Ce nombre $f'(a)$ est appelé le **nombre dérivé** de $f$ en $a$. Il correspond géométriquement au **coefficient directeur de la tangente** à la courbe au point d'abscisse $a$.

### 2. Équation de la tangente
Une équation de la tangente $T_a$ à la courbe représentative de $f$ au point d'abscisse $a$ est donnée par :
$$y = f'(a)(x - a) + f(a)$$

---

## II - Dérivation des fonctions composées

En Terminale, tu dois savoir dériver des fonctions "imbriquées" de la forme $f(u(x))$.

> [!important] Théorème général
> Si $u$ est une fonction dérivable sur $I$, et $f$ une fonction dérivable sur $J$, alors la fonction composée $f(u)$ a pour dérivée :
> $$(f(u))' = u' \times f'(u)$$

Ce théorème général donne naissance au tableau des dérivées composées usuelles à connaître **par cœur** :

| Fonction | Dérivée | Condition sur $u$ |
| :---: | :---: | :--- |
| $u^n$ ($n \in \mathbb{N}$) | $n \times u' \times u^{n-1}$ | $u$ dérivable |
| $u^2$ | $2 \times u' \times u$ | $u$ dérivable |
| $\frac{1}{u}$ | $-\frac{u'}{u^2}$ | $u \neq 0$ |
| $\sqrt{u}$ | $\frac{u'}{2\sqrt{u}}$ | $u > 0$ strictement |
| $e^u$ | $u' \times e^u$ | $u$ dérivable |
| $\ln(u)$ | $\frac{u'}{u}$ | $u > 0$ strictement |
| $\cos(u)$ | $-u' \times \sin(u)$ | $u$ dérivable |
| $\sin(u)$ | $u' \times \cos(u)$ | $u$ dérivable |

*(Rappel des règles de base : $(uv)' = u'v + uv'$ et $(\frac{u}{v})' = \frac{u'v - uv'}{v^2}$).*

---

## III - Convexité et points d'inflexion

L'étude de la convexité permet de caractériser la "courbure" d'une fonction.

### 1. Interprétation visuelle
* **Convexe** : Une fonction est convexe si sa courbe est entièrement située **au-dessus** de l'ensemble de ses tangentes.
* **Concave** : Une fonction est concave si sa courbe est entièrement située **en dessous** de l'ensemble de ses tangentes.

### 2. Le point d'inflexion
Un point d'inflexion est le point singulier où la courbe **traverse** sa tangente. C'est le point exact où la fonction change de convexité (passe de convexe à concave, ou inversement).

### 3. Caractérisation algébrique (Le Théorème)
Soit $f$ une fonction deux fois dérivable sur un intervalle $I$ (on note $f''$ sa dérivée seconde).

> [!abstract] Théorème de la convexité
> [cite_start]* $f$ est **convexe** sur $I \iff f'$ est croissante sur $I \iff f''(x) \ge 0$ sur $I$[cite: 3].
> * $f$ est **concave** sur $I \iff f'$ est décroissante sur $I \iff f''(x) \le 0$ sur $I$.
> [cite_start]* La courbe de $f$ admet un **point d'inflexion** en $a \iff f''(x)$ **s'annule en changeant de signe** en $a$[cite: 3].

---

## IV - Méthode : L'étude complète de la convexité

C'est une procédure algorithmique qui exige une grande rigueur calculatoire au baccalauréat

> [!example] Démarche pas-à-pas
> 1.  **Justifier la dérivabilité** de $f$ et dériver la fonction pour obtenir l'expression de $f'(x)$.
> 2.  **Calculer la dérivée seconde** $f''(x)$ en dérivant $f'(x)$. L'usage des formules de dérivation de produits et de quotients doit être parfaitement maîtrisé.
> 3.  **Factoriser au maximum** l'expression de $f''(x)$ pour faciliter l'étude de son signe. Dresser un tableau de signes exhaustif.
> 4.  **Rédiger la conclusion** : Sur les intervalles où $f''(x) > 0$, la fonction est convexe ; sur les intervalles où $f''(x) < 0$, elle est concave. Identifier les points d'inflexion aux abscisses où $f''$ s'annule en changeant de signe.