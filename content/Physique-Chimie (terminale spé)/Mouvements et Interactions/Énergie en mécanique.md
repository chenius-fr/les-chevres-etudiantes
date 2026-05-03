---
title: Énergie en mécanique
tags:
  - physique_chimie
  - terminale
  - cours
  - mécanique
  - énergie
  - travail
---

**Thème** : [[Mouvement et interactions]]

---

## I - Rappels et Définitions

### 1. Travail d'une force

> [!abstract] Définition : Travail d'une force
> Le travail d'une force constante $\vec{F}$ lors d'un déplacement rectiligne d'un point $A$ à un point $B$ est donné par le produit scalaire :
> $$W_{AB}(\vec{F}) = \vec{F} \cdot \vec{AB}$$
> 
> En développant le produit scalaire, on obtient :
> $$W_{AB}(\vec{F}) = F \times AB \times \cos(\alpha)$$
> *avec $\alpha$ l'angle entre le vecteur force $\vec{F}$ et le vecteur déplacement $\vec{AB}$.*
> *Le travail s'exprime en Joules (J).*

**Nature du travail (selon l'angle $\alpha$) :**
* Si $0^\circ \leq \alpha < 90^\circ$ : $\cos(\alpha) > 0$, donc $W_{AB}(\vec{F}) > 0$. Le travail est dit **moteur** (il favorise le mouvement).
* Si $90^\circ < \alpha \leq 180^\circ$ : $\cos(\alpha) < 0$, donc $W_{AB}(\vec{F}) < 0$. Le travail est dit **résistant** (il s'oppose au mouvement).
* Si $\alpha = 90^\circ$ ($\vec{F} \perp \vec{AB}$) : $\cos(\alpha) = 0$, donc $W_{AB}(\vec{F}) = 0$. Une force perpendiculaire au déplacement ne travaille pas.

> [!info] Force conservative
> Une force est dite **conservative** si son travail entre un point A et un point B ne dépend pas du chemin (trajet) suivi, mais uniquement des positions initiale et finale.
> *Exemples : le Poids ($\vec{P}$), la force électrique ($\vec{F}_E$).*

### 2. Énergie mécanique

L'énergie mécanique ($E_m$) d'un système est la somme de son énergie cinétique ($E_c$) et de son énergie potentielle ($E_p$).

> [!formula] Énergie cinétique ($E_c$)
> L'énergie cinétique est l'énergie liée à la **vitesse** d'un corps.
> $$E_c = \frac{1}{2} \cdot m \cdot v^2$$
> * $E_c$ en Joules (J)
> * $m$ la masse en kilogrammes (kg)
> * $v$ la vitesse en mètres par seconde ($\text{m}\cdot\text{s}^{-1}$)

> [!formula] Énergie potentielle de pesanteur ($E_{pp}$)
> L'énergie potentielle de pesanteur est l'énergie accumulée par un corps en raison de son **altitude** dans un champ de pesanteur.
> $$E_{pp} = m \cdot g \cdot h$$
> * $E_{pp}$ en Joules (J)
> * $m$ la masse en kilogrammes (kg)
> * $g$ l'intensité de la pesanteur ($\simeq 9,8 \text{ m}\cdot\text{s}^{-2}$)
> * $h$ l'altitude (ou $z$) en mètres (m)

> [!formula] Énergie mécanique ($E_m$)
> $$E_m = E_c + E_{pp}$$

---

## II - Les grands théorèmes énergétiques

### 1. Conservation de l'énergie mécanique

> [!important] Principe de conservation
> L'énergie mécanique d'un système se **conserve** (elle reste constante au cours du temps) si le système n'est soumis qu'à des **forces conservatives** (ou si le travail des autres forces est nul).
> $$E_{m}(A) = E_{m}(B) \iff \Delta E_m = 0$$

*Conséquence (Manuel) :* Lors d'une chute libre (où seul le poids intervient), l'énergie mécanique se conserve. Il y a une conversion totale de l'énergie potentielle en énergie cinétique lors de la descente (et inversement si l'objet est lancé vers le haut).
*(Remarque : Les forces de frottement sont dites **non-conservatives**, car elles dissipent l'énergie mécanique sous forme de chaleur).*

### 2. Théorème de l'Énergie Cinétique (TEC)

C'est l'un des théorèmes les plus puissants pour relier la vitesse aux forces appliquées, sans avoir à chercher les équations horaires du mouvement.

> [!important] Théorème de l'énergie cinétique (TEC)
> Dans un référentiel galiléen, la variation d'énergie cinétique d'un système entre un point A et un point B est égale à la somme algébrique des travaux de **toutes les forces** extérieures appliquées au système entre A et B.
> 
> $$\Delta E_{c_{A \rightarrow B}} = \sum W_{AB}(\vec{F}_{ext})$$
> 
> Soit, développé :
> $$E_c(B) - E_c(A) = W_{AB}(\vec{P}) + W_{AB}(\vec{f}) + \dots$$