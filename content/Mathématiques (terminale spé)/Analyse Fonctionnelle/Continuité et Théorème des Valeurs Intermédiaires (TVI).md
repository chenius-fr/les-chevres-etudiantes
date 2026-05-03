---
title: Continuité et Théorème des Valeurs Intermédiaires (TVI)
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - continuité
  - TVI
  - analyse
---

**Thème** : [[Analyse Fonctionnelle]]

---

## I - La notion de Continuité

### 1. Définitions (Graphique et Mathématique)
> [!abstract] Définition
> [cite_start]Graphiquement, cela signifie que la courbe d'une fonction continue peut être tracée sans lever le crayon[cite: 75].
> Mathématiquement, dire qu'une fonction $f$ est continue en un réel $a$ signifie que la limite de $f(x)$ quand $x$ tend vers $a$ est égale à l'image de $a$ :
> $$\lim_{x \to a} f(x) = f(a)$$

### 2. Fonctions de référence
* Les fonctions polynômes, rationnelles, racine carrée, exponentielle, logarithme, sinus et cosinus sont **continues sur tout intervalle où elles sont définies**.
* *Contre-exemple classique* : La fonction "Partie Entière" $E(x)$ n'est pas continue sur $\mathbb{R}$ (elle fait des "sauts" à chaque nombre entier).

---

## II - Le Théorème des Valeurs Intermédiaires (TVI)

Ce théorème est l'un des outils les plus puissants de l'analyse pour prouver l'existence de solutions à une équation.

> [!important] Théorème général
> [cite_start]Le Théorème des Valeurs Intermédiaires (TVI) garantit qu'une fonction continue prend toutes les valeurs intermédiaires entre $f(a)$ et $f(b)$[cite: 74].
> Autrement dit, si $f$ est continue sur $[a; b]$, alors pour tout réel $k$ compris entre $f(a)$ et $f(b)$, l'équation $f(x) = k$ admet **au moins une solution** dans l'intervalle $[a; b]$.

> [!danger] Corollaire du TVI (Théorème de la bijection)
> [cite_start]Son corollaire, le théorème de la bijection, ajoute la monotonie stricte pour garantir non seulement l'existence, mais surtout l'unicité d'une solution à l'équation $f(x)=k$[cite: 76]. 
> [cite_start]C'est ce corollaire [cite: 13] qui est majoritairement utilisé dans les exercices.

---

## III - Méthode : La rédaction type exigée au Bac

L'application du corollaire du TVI est systématique au baccalauréat. Les correcteurs exigent une rédaction extrêmement rigoureuse avec des mots-clés obligatoires (les mots "continue" et "strictement monotone", et l'évocation de l'encadrement des bornes).


> [!example ] Le bloc de rédaction à apprendre par cœur
> 1. "La fonction $f$ est **continue** et **strictement monotone** *(préciser croissante ou décroissante selon le tableau)* sur l'intervalle fermé $[a; b]$."
>2. "Le nombre réel $k$ *(souvent 0)* est **compris entre les valeurs $f(a)$ et $f(b)$**."
>3. "D'après le **corollaire du théorème des valeurs intermédiaires (TVI)**, l'équation $f(x) = k$ admet une **unique solution**, notée $\alpha$, sur l'intervalle $[a; b]$."