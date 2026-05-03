---
title: La fonction Logarithme Népérien
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - logarithme
  - analyse
  - limites
---

**Thème** : [[Analyse Fonctionnelle]]

---

## I - Définition et lien avec l'exponentielle

> [!abstract] Définition
> La fonction logarithme népérien, notée **$\ln$**, est définie sur l'intervalle ouvert $]0 ; +\infty[$.
> C'est la fonction réciproque de la fonction exponentielle. Elle associe à tout réel $x > 0$ l'unique antécédent de $x$ par la fonction exponentielle.

**Conséquences directes de la réciprocité :**
* Pour tout $x > 0$ et tout $y \in \mathbb{R}$ : $\quad \ln(x) = y \iff x = e^y$
* Pour tout $x \in \mathbb{R}$ : $\quad \ln(e^x) = x$
* Pour tout $x > 0$ : $\quad e^{\ln(x)} = x$

*Valeurs particulières à connaître :* $\ln(1) = 0$ et $\ln(e) = 1$.

---

## II - Propriétés algébriques fondamentales

> [!important] Règle d'or
> Là où l'exponentielle transforme les sommes en produits, **le logarithme transforme les produits en sommes**.

Pour tous réels $a > 0$ et $b > 0$, et pour tout entier $n$ :
1. **Produit :** $\ln(a \times b) = \ln(a) + \ln(b)$
2. **Quotient :** $\ln\left(\frac{a}{b}\right) = \ln(a) - \ln(b)$
3. **Inverse :** $\ln\left(\frac{1}{a}\right) = -\ln(a)$
4. **Puissance :** $\ln(a^n) = n \ln(a)$
5. **Racine carrée :** $\ln(\sqrt{a}) = \frac{1}{2} \ln(a)$

---

## III - Étude de la fonction $\ln$

### 1. Limites aux bornes et Asymptote
* $\lim_{x \to 0^+} \ln(x) = -\infty$ $\implies$ La droite d'équation **$x = 0$** (l'axe des ordonnées) est une **asymptote verticale**.
* $\lim_{x \to +\infty} \ln(x) = +\infty$

### 2. Dérivée et Variations
La fonction $\ln$ est dérivable sur $]0 ; +\infty[$ et pour tout $x > 0$ :
$$\ln'(x) = \frac{1}{x}$$
Puisque $x > 0$, la dérivée $\frac{1}{x}$ est strictement positive. La fonction logarithme est donc **strictement croissante** sur $]0 ; +\infty[$.

*Conséquences (pour les inéquations) :*
* $\ln(a) = \ln(b) \iff a = b$
* $\ln(a) < \ln(b) \iff a < b$

---

## IV - Dérivée de $\ln(u)$

> [!formula] Théorème
> Si $u$ est une fonction dérivable et **strictement positive** sur un intervalle $I$, alors la fonction $f(x) = \ln(u(x))$ est dérivable sur $I$ et sa dérivée est :
> $$f'(x) = \frac{u'(x)}{u(x)}$$

*Exemple :* $f(x) = \ln(x^2 + 5)$. On a $u(x) = x^2 + 5$ (qui est bien strictement positif) et $u'(x) = 2x$. 
Donc $f'(x) = \frac{2x}{x^2 + 5}$.

---

## V - ROC et Croissances comparées

Face aux puissances de $x$ à l'infini, le logarithme perd toujours la course (il croît extrêmement lentement).

> [!important] Limites de référence à retenir
> Pour tout entier naturel $n \ge 1$ :
> * **En $+\infty$ :** $\lim_{x \to +\infty} \frac{\ln(x)}{x^n} = 0$
> * **En $0^+$ :** $\lim_{x \to 0^+} x^n \ln(x) = 0$

> [!example] ROC : Démonstration de $\lim_{x \to 0^+} x \ln(x) = 0$
> *(Ceci est une démonstration exigible au Bac)*
> 1. On pose le changement de variable $X = \frac{1}{x}$.
> 2. Lorsque $x$ tend vers $0^+$, $X$ tend vers $+\infty$.
> 3. L'expression $x \ln(x)$ devient : $\frac{1}{X} \ln\left(\frac{1}{X}\right) = \frac{1}{X} \times (-\ln(X)) = -\frac{\ln(X)}{X}$.
> 4. Or, d'après les croissances comparées en l'infini, on sait que $\lim_{X \to +\infty} \frac{\ln(X)}{X} = 0$.
> 5. Par conséquent, $\lim_{x \to 0^+} x \ln(x) = -0 = 0$.