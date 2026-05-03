---
title: Limites de fonctions et asymptotes
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - limites
  - asymptotes
  - analyse
---

**Thème** : [[Analyse Fonctionnelle]]


---

## I - Limites en $\pm\infty$ : Définitions

### 1. Limite infinie à l'infini
> [!abstract] Définition (Intuitive et Formelle)
> Dire que $\lim_{x \to +\infty} f(x) = +\infty$ signifie que $f(x)$ peut être aussi grand que l'on veut, pourvu que $x$ soit suffisamment grand.
> 
> **Définition formelle :** Pour tout réel $A$ (aussi grand soit-il), il existe un réel $X$ tel que, pour tout $x > X$, on a $f(x) > A$.
> *(L'idée est que la courbe finit par dépasser n'importe quel seuil horizontal $A$ et y reste).*

### 2. Limite finie à l'infini (Asymptote Horizontale)
> [!important] Définition
> Dire que $\lim_{x \to +\infty} f(x) = l$ signifie que $f(x)$ devient aussi proche de $l$ que l'on veut dès que $x$ est assez grand.
> 
> **Définition formelle :** Pour tout intervalle ouvert $]l-\epsilon ; l+\epsilon[$ contenant $l$, il existe un réel $X$ tel que pour tout $x > X$, $f(x) \in ]l-\epsilon ; l+\epsilon[$.

> [!danger] Conséquence graphique
> Si $\lim_{x \to +\infty} f(x) = l$ (ou en $-\infty$), alors la droite d'équation **$y = l$** est une **asymptote horizontale** à la courbe $C_f$ au voisinage de $+\infty$.

---

## II - Limites de fonctions de référence

Voici les limites à connaître par cœur pour lever les formes indéterminées :

| Fonction $f(x)$ | Limite en $+\infty$ | Limite en $-\infty$ |
| :--- | :--- | :--- |
| $x, x^2, x^n$ ($n$ pair) | $+\infty$ | $+\infty$ |
| $x^n$ ($n$ impair) | $+\infty$ | $-\infty$ |
| $\sqrt{x}$ | $+\infty$ | *(Non définie)* |
| $1/x, 1/x^n, 1/\sqrt{x}$ | $0$ | $0$ |

---

## III - Limite infinie en un réel $a$ (Asymptote Verticale)

> [!abstract] Définition
> Dire que $\lim_{x \to a} f(x) = +\infty$ signifie que les valeurs de $f(x)$ deviennent arbitrairement grandes dès que $x$ se rapproche suffisamment de $a$.

> [!danger] Conséquence graphique
> Si $\lim_{x \to a} f(x) = \pm\infty$, alors la droite d'équation **$x = a$** est une **asymptote verticale** à la courbe $C_f$.

*Note : On distingue souvent la limite à gauche ($x \to a^-$) et la limite à droite ($x \to a^+$).*

---

## IV - Opérations et formes indéterminées

Les règles de calcul sont intuitives (ex: $+\infty + (+\infty) = +\infty$), sauf dans 4 cas critiques appelés **Formes Indéterminées (FI)** :

1. **La somme :** $(+\infty) + (-\infty)$
2. **Le produit :** $0 \times \infty$
3. **Le quotient :** $\frac{\infty}{\infty}$
4. **Le quotient :** $\frac{0}{0}$

> [!tip] Méthodes pour lever une FI
> * **Pour les polynômes/fractions rationnelles à l'infini** : On factorise par le terme de plus haut degré.
> * **Pour les racines carrées** : On utilise l'expression conjuguée ou la factorisation forcée sous la racine.
> * **Pour les limites de cours** : On utilise les croissances comparées (voir chapitres suivants).

---

## V - Théorèmes de comparaison et de composition

### 1. Théorème des Gendarmes
Si $g(x) \le f(x) \le h(x)$ et si $\lim_{x \to a} g(x) = \lim_{x \to a} h(x) = l$, alors **$\lim_{x \to a} f(x) = l$**.

### 2. Théorèmes de comparaison (Infinis)
* Si $f(x) \ge g(x)$ et $\lim_{x \to a} g(x) = +\infty$, alors **$\lim_{x \to a} f(x) = +\infty$**.
* Si $f(x) \le g(x)$ et $\lim_{x \to a} g(x) = -\infty$, alors **$\lim_{x \to a} f(x) = -\infty$**.

### 3. Limite d'une fonction composée
> [!formula] Théorème
> Soient deux fonctions $u$ et $v$. Pour trouver $\lim_{x \to a} v(u(x))$ :
> 1. On calcule d'abord $\lim_{x \to a} u(x) = b$.
> 2. On calcule ensuite $\lim_{X \to b} v(X) = L$.
> 3. Alors $\lim_{x \to a} v(u(x)) = L$.