---
title: Inégalité de Bienaymé-Tchebychev et Concentration
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - probabilités
  - concentration
  - statistiques
---

**Thème** : [[Probabilités]]

---

## I - L'inégalité de Markov

L'inégalité de Markov est un résultat préliminaire qui concerne uniquement les variables aléatoires positives. Elle affirme que la probabilité qu'une variable prenne de très grandes valeurs est limitée par son espérance.

> **Théorème (Inégalité de Markov)**
> Soit $X$ une variable aléatoire à valeurs **positives** admettant une espérance $E(X)$.
> Pour tout réel $a > 0$, on a :
> $$P(X \ge a) \le \frac{E(X)}{a}$$

*Exemple intuitif : Si le salaire moyen dans une entreprise est de 2000€, la proportion d'employés gagnant plus de 6000€ ($a = 6000$) ne peut pas dépasser $2000 / 6000 = 1/3$.*

---

## II - L'inégalité de Bienaymé-Tchebychev

C'est le cœur du chapitre. Cette inégalité s'applique à **n'importe quelle variable aléatoire** (pas seulement positive), à condition de connaître son espérance $\mu = E(X)$ et sa variance $V(X)$. 

Elle permet de majorer la probabilité que la variable s'éloigne "trop" de sa moyenne.

> **Théorème (Inégalité de Bienaymé-Tchebychev)**
> Soit $X$ une variable aléatoire d'espérance $\mu$ et de variance $V(X)$.
> Pour tout réel strictement positif $\delta$ (delta), on a :
> $$P(|X - \mu| \ge \delta) \le \frac{V(X)}{\delta^2}$$

**Interprétation :** L'expression $|X - \mu| \ge \delta$ signifie "l'écart entre $X$ et sa moyenne est supérieur ou égal à $\delta$". Le théorème garantit que la probabilité qu'une telle "déviation" se produise est plafonnée par $\frac{V(X)}{\delta^2}$.

---

## III - Le phénomène de Concentration

En passant à l'événement contraire, l'inégalité de Bienaymé-Tchebychev nous donne une garantie sur la probabilité que $X$ reste **proche** de sa moyenne. C'est ce qu'on appelle la concentration.

> **Formule de la concentration**
> Pour tout réel $\delta > 0$ :
> $$P(|X - \mu| < \delta) \ge 1 - \frac{V(X)}{\delta^2}$$

---

## IV - Rédaction type (Tirée des annales du Bac)

Voici la méthode de rédaction rigoureuse attendue au baccalauréat pour justifier un encadrement probabiliste. 

**Énoncé type :** Une machine produit des pièces. Le poids $X$ d'une pièce a pour espérance $\mu = 500$ g et pour variance $V(X) = 400$. Quelle est la probabilité que le poids s'écarte de plus de 50 g de la moyenne ? Quelle est la probabilité qu'il reste dans cet intervalle ?

> **1. Majoration de l'écart (Inégalité stricte) :**
> On cherche $P(|X - 500| \ge 50)$. On applique l'inégalité de Bienaymé-Tchebychev avec $\delta = 50$ :
> $$P(|X - 500| \ge 50) \le \frac{V(X)}{\delta^2}$$
> $$P(|X - 500| \ge 50) \le \frac{400}{50^2}$$
> $$P(|X - 500| \ge 50) \le \frac{400}{2500} \le 0,16$$
> *Conclusion : Le risque d'observer un écart supérieur à 50g est plafonné à 16%.*

> **2. Minoration de la normalité (Événement contraire) :**
> L'événement "le poids reste à moins de 50g de la moyenne" s'écrit $|X - 500| < 50$. Il s'agit de l'événement contraire du précédent.
> La somme des probabilités valant 1, on a :
> $$P(|X - 500| < 50) = 1 - P(|X - 500| \ge 50)$$
> Puisque $P(|X - 500| \ge 50) \le 0,16$, en soustrayant on inverse l'inégalité :
> $$P(|X - 500| < 50) \ge 1 - 0,16$$
> $$P(|X - 500| < 50) \ge 0,84$$
> *Conclusion : La probabilité que la production reste dans la norme est d'au moins 84%.*