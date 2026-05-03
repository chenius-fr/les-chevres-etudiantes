---
title: Équations différentielles et Primitives
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - primitives
  - équa_diff
  - analyse
---

**Thème** : [[Calcul Intégral et Équations Différentielles]]

---

## I - Notion de Primitive

### 1. Définition
> [!abstract] Définition
> Soit $f$ une fonction continue sur un intervalle $I$. 
> On appelle **primitive** de $f$ sur $I$ toute fonction $F$ dérivable sur $I$ telle que pour tout $x \in I$ :
> $$F'(x) = f(x)$$

### 2. Ensemble des primitives et condition initiale
* **Infinité :** Si $F$ est une primitive de $f$, alors toutes les fonctions de la forme $G(x) = F(x) + k$ (où $k \in \mathbb{R}$) sont aussi des primitives de $f$.
* **Unicité (Corollaire) :** Pour tout réel $x_0 \in I$ et tout réel $y_0$, il existe une **unique** primitive $F_0$ vérifiant la condition initiale $F_0(x_0) = y_0$.
*(Méthode : On trouve l'expression générale avec le $+ k$, puis on résout l'équation pour trouver la valeur exacte de la constante $k$).*

---

## II - Tableaux des Primitives

La recherche de primitives demande de lire le tableau des dérivées "à l'envers".

### 1. Primitives usuelles (avec $k \in \mathbb{R}$)

| Fonction $f(x)$ | Une primitive $F(x)$ |
| :--- | :--- |
| $a$ (constante) | $ax + k$ |
| $x^n$ ($n \in \mathbb{N}$) | $\frac{x^{n+1}}{n+1} + k$ |
| $\frac{1}{x^n}$ ($n \ge 2$) | $-\frac{1}{(n-1)x^{n-1}} + k$ |
| $\frac{1}{\sqrt{x}}$ | $2\sqrt{x} + k$ |
| $e^x$ | $e^x + k$ |
| $\cos(x)$ | $\sin(x) + k$ |
| $\sin(x)$ | $-\cos(x) + k$ |

### 2. Formes composées (Indispensable au Bac)
Pour trouver la primitive d'une fonction composée, il faut faire apparaître la dérivée $u'$ devant la fonction.

| Forme de $f$ | Forme des primitives $F$ |
| :--- | :--- |
| $u' \times u^n$ | $\frac{u^{n+1}}{n+1} + k$ |
| $\frac{u'}{u^2}$ | $-\frac{1}{u} + k$ |
| $\frac{u'}{\sqrt{u}}$ | $2\sqrt{u} + k$ |
| $u' \times e^u$ | $e^u + k$ |
| $u' \times \cos(u)$ | $\sin(u) + k$ |
| $u' \times \sin(u)$ | $-\cos(u) + k$ |

*(Astuce de calcul : N'hésite pas à multiplier et diviser par une même constante pour faire apparaître le bon $u'$).*

---

## III - Équations différentielles linéaires du 1er ordre

Une équation différentielle est une équation dont l'inconnue n'est pas un nombre $x$, mais une fonction $y$ (et on y trouve sa dérivée $y'$).

### 1. Équation du type $y' = ay$
> [!important] Théorème
> Les solutions de l'équation différentielle $y' = ay$ (avec $a \in \mathbb{R}$) sont les fonctions de la forme :
> $$f(x) = C \cdot e^{ax}$$
> où $C$ est une constante réelle.

### 2. Équation du type $y' = ay + b$
> [!important] Théorème
> Les solutions de l'équation différentielle $y' = ay + b$ (avec $a \neq 0$) sont les fonctions de la forme :
> $$f(x) = C \cdot e^{ax} - \frac{b}{a}$$
> où $C$ est une constante réelle.

### 3. Résolution d'équations plus complexes $y' = ay + f(x)$
Dans les sujets de bac, on procède en trois étapes guidées :
1. On te donne une **solution particulière** $g(x)$ que tu dois vérifier (en dérivant $g$ et en l'injectant dans l'équation).
2. On démontre qu'une fonction $h$ est solution de l'équation complète **si et seulement si** la fonction $(h - g)$ est solution de l'équation sans second membre ($y' = ay$).
3. On utilise le théorème du cours pour trouver $(h - g)$, puis on en déduit l'expression finale de $h$.