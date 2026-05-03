---
title: Vecteurs, droites et plans dans l'espace
draft: false
tags:
  - mathématiques
  - terminale
  - cours
  - géométrie
  - espace
  - vecteurs
---

**Thème** : [[Algèbre et Géométrie]]

---

## I - Vecteurs et repérage dans l'espace

L'espace est rapporté à un repère orthonormé $(O; \vec{i}, \vec{j}, \vec{k})$. Un point $M$ ou un vecteur $\vec{u}$ est défini par trois coordonnées : l'abscisse $x$, l'ordonnée $y$ et la cote $z$.

> **Coordonnées d'un vecteur et distance**
> * Pour deux points $A(x_A, y_A, z_A)$ et $B(x_B, y_B, z_B)$, le vecteur $\vec{AB}$ a pour coordonnées : 
>   $$\vec{AB} \begin{pmatrix} x_B - x_A \\ y_B - y_A \\ z_B - z_A \end{pmatrix}$$
> * La distance $AB$ (ou norme du vecteur) est :
>   $$AB = \sqrt{(x_B - x_A)^2 + (y_B - y_A)^2 + (z_B - z_A)^2}$$

**Colinéarité et Coplanarité :**
* Deux vecteurs sont **colinéaires** si et seulement si leurs coordonnées sont proportionnelles (ils ont la même direction).
* Trois vecteurs sont **coplanaires** si l'un peut s'écrire comme une combinaison linéaire des deux autres (ex: $\vec{w} = a\vec{u} + b\vec{v}$). Ils appartiennent alors à un même plan.

---

## II - Le Produit Scalaire dans l'espace

Le produit scalaire est l'outil absolu pour démontrer que des éléments sont perpendiculaires (orthogonaux).

> **Expression analytique**
> Dans un repère orthonormé, le produit scalaire de deux vecteurs $\vec{u}(x, y, z)$ et $\vec{v}(x', y', z')$ se calcule ainsi :
> $$\vec{u} \cdot \vec{v} = xx' + yy' + zz'$$

> **Orthogonalité (Le test fondamental)**
> Deux vecteurs $\vec{u}$ et $\vec{v}$ sont orthogonaux si et seulement si leur produit scalaire est nul :
> $$\vec{u} \cdot \vec{v} = 0$$

---

## III - Droites et Plans : Les équations

Dans l'espace, une droite et un plan ne se définissent pas du tout de la même manière mathématique.

### 1. Représentation paramétrique d'une droite
Une droite $\mathcal{D}$ est définie par un point $A(x_A, y_A, z_A)$ et un vecteur directeur $\vec{u}(a, b, c)$.
Un point $M(x, y, z)$ appartient à la droite $\mathcal{D}$ s'il existe un réel $t$ (le paramètre) tel que $\vec{AM} = t\vec{u}$.

> **Système paramétrique**
> $$\begin{cases} x = x_A + a \cdot t \\ y = y_A + b \cdot t \\ z = z_A + c \cdot t \end{cases} \quad \text{avec } t \in \mathbb{R}$$

### 2. Équation cartésienne d'un plan
Un plan $\mathcal{P}$ est défini par un point et **deux** vecteurs directeurs, OU plus simplement par un point et **un vecteur normal** $\vec{n}$.
Un vecteur normal à un plan est un vecteur non nul qui est orthogonal à tous les vecteurs de ce plan.

> **Théorème de l'équation cartésienne**
> Le plan de vecteur normal $\vec{n}(a, b, c)$ admet une équation cartésienne de la forme :
> $$ax + by + cz + d = 0$$
> *(Pour trouver la valeur de $d$, il suffit de remplacer $x, y, z$ par les coordonnées d'un point appartenant au plan).*

---

## IV - Intersections et Problèmes classiques

Au baccalauréat, on vous demande souvent de trouver l'intersection entre différents objets. La méthode consiste toujours à **résoudre un système d'équations**.

* **Intersection d'une droite et d'un plan :**
  On remplace les expressions de $x, y, z$ de la représentation paramétrique de la droite directement dans l'équation cartésienne du plan. On obtient une équation à une seule inconnue : le paramètre $t$. Une fois $t$ trouvé, on réinjecte sa valeur pour trouver les coordonnées du point d'intersection.
* **Projeté orthogonal d'un point sur un plan :**
  Pour trouver le projeté orthogonal $H$ d'un point $A$ sur un plan $\mathcal{P}$ :
  1. On crée la droite $\mathcal{D}$ passant par $A$ et de vecteur directeur $\vec{n}$ (le vecteur normal du plan).
  2. On cherche l'intersection entre cette droite $\mathcal{D}$ et le plan $\mathcal{P}$. Le point trouvé est $H$.