---
title: Calcul Intégral
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - intégrale
  - analyse
  - aire
---

**Thème** : [[Calcul Intégral et Équations Différentielles]]


---

## I - Intégrale et Primitives : Le calcul fondamental

Jusqu'à présent, nous trouvions des fonctions "générales" (les primitives). L'intégrale permet d'obtenir un **nombre réel** précis en évaluant cette primitive entre deux bornes.

> **Théorème fondamental du calcul intégral**
> Soit $f$ une fonction continue sur un intervalle $I$, et $a$ et $b$ deux réels de $I$. 
> Si $F$ est une primitive de $f$ sur $I$, alors l'intégrale de $f$ entre $a$ et $b$ est le nombre réel défini par :
> $$\int_{a}^{b} f(x) dx = \left[ F(x) \right]_{a}^{b} = F(b) - F(a)$$

**Remarque importante :** Le résultat de l'intégrale ne dépend absolument pas de la primitive choisie (la constante $k$ s'annule lors de la soustraction $F(b) - F(a)$).

**Propriétés des crochets de variation :**
* Pour une constante $k$ : $\left[ k \cdot F(x) \right]_{a}^{b} = k \cdot \left[ F(x) \right]_{a}^{b}$
* Pour une somme : $\left[ (F+G)(x) \right]_{a}^{b} = \left[ F(x) \right]_{a}^{b} + \left[ G(x) \right]_{a}^{b}$

---

## II - Interprétation graphique : L'aire sous la courbe

Le calcul intégral a été inventé historiquement pour calculer des aires de surfaces délimitées par des courbes.

### 1. Fonction positive (Aire géométrique)
Si $f$ est une fonction **continue et positive** sur $[a ; b]$ (avec $a < b$), alors $\int_{a}^{b} f(x) dx$ correspond exactement à l'aire du domaine délimité par :
* La courbe représentative de $f$
* L'axe des abscisses
* Les droites verticales d'équations $x = a$ et $x = b$
Le résultat s'exprime en **Unités d'Aire (u.a.)**.

### 2. Fonction de signe quelconque (Aire algébrique)
L'intégrale calcule une aire "algébrique" :
* Les domaines situés **au-dessus** de l'axe des abscisses sont comptés **positivement**.
* Les domaines situés **en dessous** de l'axe des abscisses sont comptés **négativement**.
*L'intégrale globale est donc la somme de ces aires algébriques.*

---

## III - Propriétés de l'intégrale

Ces propriétés permettent de simplifier grandement les calculs au baccalauréat.

1. **Inversion des bornes :** $$\int_{b}^{a} f(x) dx = - \int_{a}^{b} f(x) dx$$
2. **Intégrale nulle :**
   $$\int_{a}^{a} f(x) dx = 0$$
3. **Relation de Chasles :** Pour tout point $c$ situé entre $a$ et $b$ :
   $$\int_{a}^{b} f(x) dx = \int_{a}^{c} f(x) dx + \int_{c}^{b} f(x) dx$$
4. **Linéarité :** L'intégrale d'une somme est la somme des intégrales, et on peut sortir les constantes multiplicatives de l'intégrale :
   $$\int_{a}^{b} (\alpha f(x) + \beta g(x)) dx = \alpha \int_{a}^{b} f(x) dx + \beta \int_{a}^{b} g(x) dx$$

---

## IV - Valeur moyenne d'une fonction

La valeur moyenne correspond à la hauteur constante d'un rectangle de base $(b-a)$ qui aurait exactement la même aire que le domaine sous la courbe de $f$.

> **Formule de la valeur moyenne**
> Soit $f$ une fonction continue sur l'intervalle $[a ; b]$ (avec $a < b$). 
> La valeur moyenne de la fonction $f$ sur cet intervalle est le réel $\mu$ défini par :
> $$\mu = \frac{1}{b-a} \int_{a}^{b} f(x) dx$$