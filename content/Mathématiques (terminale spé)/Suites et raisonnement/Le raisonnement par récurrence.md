---
title: Le raisonnement par récurrence
draft: false
tags:
  - "#mathématiques"
  - terminale
  - cours
  - suites
  - récurrence
---

**Thème** : [[Suites et Raisonnement]]

---

## I - Le principe du raisonnement par récurrence

> [!info] Principe fondamental
> Le raisonnement par récurrence est le fondement de la démonstration mathématique pour les propositions dépendant d'un entier naturel $n$. Il permet de prouver qu'une proposition $P_n$ est vraie pour tout entier $n \ge n_0$ (où $n_0$ est l'entier de départ).

La démonstration s'effectue **obligatoirement** en trois étapes distinctes et rigoureuses :

### 1. L'Initialisation
On vérifie que la proposition est vraie pour le tout premier rang (l'entier fixé $n_0$). 
*Exemple : Si l'on doit prouver une propriété pour tout $n \ge 10$, l'initialisation se fait en remplaçant $n$ par $10$ dans l'égalité ou l'inégalité.*

### 2. L'Hérédité
On suppose que la proposition est vraie pour un rang $k$ fixé arbitrairement (avec $k \ge n_0$). Cette supposition est appelée **l'hypothèse de récurrence (HR)**.
L'objectif est de démontrer, en manipulant algébriquement l'expression et en utilisant l'HR, que la proposition est inévitablement vraie au rang suivant ($k+1$).

### 3. La Conclusion
On clôture la démonstration par une phrase rituelle certifiant que les deux étapes précédentes valident la propriété pour tout $n$.

---

## II - Exemple de rédaction type (Type Bac)

**Objectif :** Démontrer par récurrence que pour tout entier naturel $n \ge 10$, on a $2^n \ge 100n$.

Soit $P_n$ la proposition : "$2^n \ge 100n$".

> [!example] 1. Initialisation
> Pour $n = 10$ :
> D'une part, $2^{10} = 1024$.
> D'autre part, $100 \times 10 = 1000$.
> On constate que $1024 \ge 1000$, donc $2^{10} \ge 100 \times 10$.
> **La proposition $P_{10}$ est vraie.**

> [!example] 2. Hérédité
> Soit $k$ un entier naturel tel que $k \ge 10$. 
> Supposons que la proposition $P_k$ est vraie, c'est-à-dire que **$2^k \ge 100k$** *(Hypothèse de récurrence)*.
> Démontrons sous cette condition que $P_{k+1}$ est vraie, c'est-à-dire que **$2^{k+1} \ge 100(k+1)$** (soit $2^{k+1} \ge 100k + 100$).
>
> Par hypothèse de récurrence :
> $$2^k \ge 100k$$
> En multipliant les deux membres par 2 (qui est $> 0$, l'ordre est conservé) :
> $$2 \times 2^k \ge 2 \times 100k$$
> $$2^{k+1} \ge 200k$$
>
> Or, on sait que $200k = 100k + 100k$.
> Puisque $k \ge 10$, on a $100k \ge 1000 \ge 100$.
> Il en découle que $200k \ge 100k + 100$.
>
> Par transitivité des inégalités, on obtient donc :
> $$2^{k+1} \ge 100k + 100$$
> $$2^{k+1} \ge 100(k+1)$$
> **La proposition est héréditaire.**

> [!example] 3. Conclusion
> La propriété $P_n$ est initialisée au rang $n=10$ et est héréditaire. D'après le principe de récurrence, on conclut qu'elle est vraie pour tout entier naturel $n \ge 10$.

---

## III - ROC : L'Inégalité de Bernoulli

L'inégalité de Bernoulli est une démonstration classique exigible au baccalauréat. Elle établit une minoration puissante pour les puissances.

> [!important] Théorème (Inégalité de Bernoulli)
> Pour tout réel $a > 0$ et pour tout entier naturel $n$ :
> $$(1+a)^n \ge 1+na$$

*(Rappel méthodologique : Sa démonstration s'effectue par récurrence, en multipliant l'hypothèse de récurrence par le facteur positif $(1+a)$ pour passer au rang $k+1$, puis en développant et en ignorant le terme positif $k \cdot a^2$).*