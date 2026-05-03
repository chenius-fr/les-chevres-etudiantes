---
title: Fonctions trigonométriques (Sinus et Cosinus)
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - trigonométrie
  - fonctions
  - analyse
---

**Thème** : [[Analyse Fonctionnelle]]

---

## I - Définitions et Cercle Trigonométrique

Le plan est rapporté à un repère orthonormé $(O;\vec{i},\vec{j})$. Le cercle trigonométrique est le cercle de centre $O$ et de rayon $1$, orienté dans le sens direct (anti-horaire).
À tout réel $x$ (exprimé obligatoirement en **radians**), on associe un unique point $M$ sur le cercle.
* **$\cos(x)$** est l'abscisse du point $M$.
* **$\sin(x)$** est l'ordonnée du point $M$.

**Propriétés fondamentales :**
* Pour tout réel $x$ : $-1 \le \cos(x) \le 1$ et $-1 \le \sin(x) \le 1$
* Relation fondamentale : $\cos^2(x) + \sin^2(x) = 1$
* Périodicité basique : $\cos(x + 2k\pi) = \cos(x)$ et $\sin(x + 2k\pi) = \sin(x)$ (avec $k \in \mathbb{Z}$)

---

## II - Formules de Trigonométrie

### 1. Angles associés (Symétries du cercle)
* **Angle opposé** : $\cos(-x) = \cos(x)$ et $\sin(-x) = -\sin(x)$
* **Demi-tour** : $\cos(\pi - x) = -\cos(x)$ et $\sin(\pi - x) = \sin(x)$
* **Demi-tour + x** : $\cos(\pi + x) = -\cos(x)$ et $\sin(\pi + x) = -\sin(x)$

### 2. Formules d'addition et de duplication
Ces formules permettent de développer des expressions :
* $\cos(a+b) = \cos(a)\cos(b) - \sin(a)\sin(b)$
* $\cos(a-b) = \cos(a)\cos(b) + \sin(a)\sin(b)$
* $\sin(a+b) = \sin(a)\cos(b) + \sin(b)\cos(a)$
* $\sin(a-b) = \sin(a)\cos(b) - \sin(b)\cos(a)$

**Formules de duplication (cas où $a = b$) :**
* $\sin(2a) = 2\sin(a)\cos(a)$
* $\cos(2a) = \cos^2(a) - \sin^2(a) = 2\cos^2(a) - 1 = 1 - 2\sin^2(a)$

---

## III - Étude des fonctions sinus et cosinus

### 1. Parité et Périodicité
* **Périodicité** : Les fonctions $\cos$ et $\sin$ sont périodiques de période $2\pi$. On peut donc restreindre leur étude à un intervalle de longueur $2\pi$ (souvent $[-\pi ; \pi]$).
* **Parité** : 
    * La fonction $\cos$ est **paire** ($\cos(-x) = \cos(x)$). Sa courbe est symétrique par rapport à l'axe des ordonnées.
    * La fonction $\sin$ est **impaire** ($\sin(-x) = -\sin(x)$). Sa courbe est symétrique par rapport à l'origine du repère.

### 2. Dérivation
Les fonctions sinus et cosinus sont dérivables sur $\mathbb{R}$.
* $(\sin(x))' = \cos(x)$
* $(\cos(x))' = -\sin(x)$

*(Remarque : La démonstration de cette dérivée avec le taux d'accroissement utilise les limites de référence $\lim_{x \to 0} \frac{\sin(x)}{x} = 1$ et $\lim_{x \to 0} \frac{\cos(x) - 1}{x} = 0$).*

---

## IV - Équations et Inéquations trigonométriques

Pour résoudre ces équations, il faut systématiquement tracer un petit cercle trigonométrique au brouillon pour ne rater aucune solution.

### 1. Équations
* **Équation $\cos(x) = \cos(a)$** :
  Les solutions sont $x = a + 2k\pi$ **OU** $x = -a + 2k\pi$ (avec $k \in \mathbb{Z}$).
* **Équation $\sin(x) = \sin(a)$** :
  Les solutions sont $x = a + 2k\pi$ **OU** $x = \pi - a + 2k\pi$ (avec $k \in \mathbb{Z}$).

### 2. Inéquations
Méthode générale pour résoudre une inéquation (ex: $\cos(x) > 0,5$ sur $[-\pi ; \pi]$) :
1. On place la valeur cible sur l'axe correspondant (abscisses pour le cosinus, ordonnées pour le sinus).
2. On trace la ligne orthogonale correspondante pour marquer les points d'intersection avec le cercle.
3. On surligne l'arc de cercle qui vérifie l'inégalité.
4. On lit l'intervalle solution en tournant dans le sens trigonométrique (sens anti-horaire).