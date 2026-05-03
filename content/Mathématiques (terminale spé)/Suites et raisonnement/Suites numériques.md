---
title: Suites numériques
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - suites
  - limites
  - convergence
---

**Thème** : [[Suites et Raisonnement]]

---

## I - Rappels et définitions

### 1. Définition et notations
Une suite réelle $u$ est une fonction définie sur $\mathbb{N}$ (ou à partir d'un certain rang $n_0$). On note $u_n$ l'image de l'entier $n$, appelée **terme de rang $n$**.

Il existe deux manières principales de définir une suite :
* **Forme explicite** : $u_n = f(n)$. Chaque terme se calcule directement en fonction de $n$.
* **Forme par récurrence** : $u_{n+1} = f(u_n)$. Chaque terme se calcule à partir du précédent (nécessite un premier terme $u_0$).

### 2. Sens de variation (Monotonie)
Pour étudier le sens de variation d'une suite $(u_n)$, on étudie généralement le signe de la différence $u_{n+1} - u_n$ :
* Si $u_{n+1} - u_n \ge 0$, la suite est **croissante**.
* Si $u_{n+1} - u_n \le 0$, la suite est **décroissante**.

### 3. Suites majorées, minorées et bornées
> [!abstract] Définitions
> * **Majorée** : Il existe un réel $M$ tel que pour tout $n$, $u_n \le M$.
> * **Minorée** : Il existe un réel $m$ tel que pour tout $n$, $u_n \ge m$.
> * **Bornée** : La suite est à la fois majorée et minorée.

---

## II - Suites de référence

### 1. Suites Arithmétiques
* **Définition** : $u_{n+1} = u_n + r$ ($r$ est la raison).
* **Terme général** : $u_n = u_p + (n-p)r$.
* **Somme de termes consécutifs** : $S = \text{nb de termes} \times \frac{\text{premier} + \text{dernier}}{2}$.

### 2. Suites Géométriques
* **Définition** : $u_{n+1} = u_n \times q$ ($q$ est la raison).
* **Terme général** : $u_n = u_p \times q^{n-p}$.
* **Somme de termes consécutifs** ($q \neq 1$) : $S = \text{premier terme} \times \frac{1 - q^{\text{nb de termes}}}{1 - q}$.

---

## III - Limites de suites

### 1. Limite finie et Convergence
> [!important] Définition (Intervalle ouvert)
> On dit qu'une suite $(u_n)$ a pour limite $l$ si tout intervalle ouvert contenant $l$ contient tous les termes de la suite à partir d'un certain rang.
> On note : $\lim_{n \to +\infty} u_n = l$. La suite est dite **convergente**.

### 2. Limite infinie et Divergence
> [!important] Définition ($+\infty$)
> On dit qu'une suite $(u_n)$ a pour limite $+\infty$ si tout intervalle $]A ; +\infty[$ contient tous les termes de la suite à partir d'un certain rang.
> La suite est alors **divergente**.

### 3. Opérations sur les limites
Les règles de calcul sont les mêmes que pour les fonctions.
* **Formes Indéterminées (FI)** : "$+\infty - \infty$", "$0 \times \infty$", "$\frac{\infty}{\infty}$", "$\frac{0}{0}$".

---

## IV - Théorèmes de comparaison et de convergence

### 1. Théorèmes de comparaison
Soient $(u_n)$ et $(v_n)$ deux suites telles qu'à partir d'un certain rang $n \ge p$ :
* Si $u_n \le v_n$ et $\lim u_n = +\infty$, alors $\lim v_n = +\infty$.
* Si $u_n \le v_n$ et $\lim v_n = -\infty$, alors $\lim u_n = -\infty$.

### 2. Théorème des Gendarmes
Si $v_n \le u_n \le w_n$ et $\lim v_n = \lim w_n = l$, alors $\lim u_n = l$.

### 3. Théorème de convergence monotone
* Toute suite **croissante et majorée** converge vers une limite finie $l$.
* Toute suite **décroissante et minorée** converge vers une limite finie $l$.
* Si une suite est **croissante et non majorée**, elle diverge vers $+\infty$.

---

## V - ROC : Limite de la suite géométrique $q^n$

C'est une démonstration exigible au bac (Restitution Organisée de Connaissances).

> [!theory] Propriété
> Soit $q$ un réel.
> * Si $q > 1$, alors $\lim_{n \to +\infty} q^n = +\infty$.
> * Si $-1 < q < 1$, alors $\lim_{n \to +\infty} q^n = 0$.
> * Si $q \le -1$, la suite n'a pas de limite.

**Démonstration pour $q > 1$ :**
1. On pose $q = 1 + a$ avec $a > 0$ (puisque $q > 1$).
2. D'après l'inégalité de Bernoulli : $(1+a)^n \ge 1 + na$.
3. Comme $a > 0$, $\lim_{n \to +\infty} (1+na) = +\infty$.
4. Par comparaison, on en déduit que $\lim_{n \to +\infty} (1+a)^n = +\infty$, soit $\lim_{n \to +\infty} q^n = +\infty$.