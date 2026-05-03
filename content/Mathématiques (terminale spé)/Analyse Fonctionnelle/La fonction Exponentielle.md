---
title: La fonction Exponentielle
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - exponentielle
  - analyse
  - limites
---

**Thème** : [[Analyse Fonctionnelle]]
**Tags** : #mathématiques #terminale #cours #exponentielle #analyse #limites

---

## I - Définition et Propriétés algébriques

### 1. Définition
On admet qu'il existe une unique fonction $f$, dérivable sur $\mathbb{R}$, telle que :
$$f'(x) = f(x) \quad \text{et} \quad f(0) = 1$$
Cette fonction est appelée **fonction exponentielle**, notée $\exp$. 
Pour tout réel $x$, on pose $\exp(x) = e^x$, où $e \approx 2,72$ est l'image de 1.

### 2. Propriétés algébriques fondamentales
La fonction exponentielle transforme les sommes en produits. Pour tous réels $x$ et $y$, et tout entier relatif $n$ :
* $e^{x+y} = e^x \times e^y$
* $e^{-x} = \frac{1}{e^x}$
* $e^{x-y} = \frac{e^x}{e^y}$
* $(e^x)^n = e^{nx}$

---

## II - Étude de la fonction exponentielle

### 1. Signe et Variations
> [!danger] Règle d'or absolue
> Pour tout réel $x$, on a strictement : **$e^x > 0$**
> L'exponentielle n'est **jamais nulle** et **jamais négative**.

Puisque sa dérivée est elle-même ($f'(x) = e^x$) et que $e^x > 0$, la fonction exponentielle est **strictement croissante** sur $\mathbb{R}$.

Conséquences de la stricte croissance (très utiles pour résoudre des équations/inéquations) :
* $e^a = e^b \iff a = b$
* $e^a < e^b \iff a < b$

### 2. Tangente à l'origine
L'équation de la tangente à la courbe en $x=0$ est $y = x + 1$. 
Par un argument de convexité (la courbe de l'exponentielle est toujours au-dessus de ses tangentes), on a pour tout réel $x$ : **$e^x \ge x + 1$**.

---

## III - Limites et Croissances comparées

### 1. Limites aux bornes (Cours)
* $\lim_{x \to -\infty} e^x = 0$ (Asymptote horizontale $y=0$ en $-\infty$)
* $\lim_{x \to +\infty} e^x = +\infty$

### 2. Croissances comparées (Théorème fondamental)
Face à une forme indéterminée mélangeant des polynômes ($x^n$) et l'exponentielle ($e^x$) à l'infini, **l'exponentielle l'emporte toujours**.

> [!important] Formules de croissances comparées à connaître par cœur
> Pour tout entier naturel $n \ge 1$ :
> * **En $+\infty$ :** $\lim_{x \to +\infty} \frac{e^x}{x^n} = +\infty$
> * **En $-\infty$ :** $\lim_{x \to -\infty} x^n e^x = 0$

*Note : Une limite classique liée au taux d'accroissement en 0 est également à retenir : $\lim_{x \to 0} \frac{e^x - 1}{x} = 1$.*

---

## IV - Dérivation de fonctions composées $e^{u(x)}$

C'est la forme la plus courante dans les exercices du baccalauréat.

> [!formula] Théorème
> Si $u$ est une fonction dérivable sur un intervalle $I$, alors la fonction $f(x) = e^{u(x)}$ est dérivable sur $I$ et sa dérivée est :
> $$f'(x) = u'(x) \times e^{u(x)}$$

**Exemple d'application type :** Soit $f(x) = e^{-x^2+3x}$. On a $u(x) = -x^2+3x$, donc $u'(x) = -2x+3$.
La dérivée est donc $f'(x) = (-2x+3)e^{-x^2+3x}$.
*(Pour étudier le signe de $f'$, il suffira d'étudier le signe de $-2x+3$ puisque l'exponentielle est toujours strictement positive !)*