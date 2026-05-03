# Chapitre 11 : La lunette astronomique
**Thème** : [[Ondes et signaux]]
**Tags** : #physique_chimie #terminale #cours #optique #lunette_astronomique

---

## I - Rappels sur les lentilles minces

> [!info] Définition
> Les lentilles sont des dispositifs d'optique permettant de dévier la lumière en utilisant le phénomène de réfraction.
> Il en existe deux types :
> * **Convergentes (CV)** : Effet loupe, bombées au milieu et fines sur les bords. Symbole : $\updownarrow$
> * **Divergentes (DV)** : Effet loupe "inversé", creuses au milieu et épaisses sur les bords.

### 1. Propriétés des lentilles convergentes

> [!abstract] Vocabulaire de l'optique géométrique
> * **Centre optique ($O$)** : Centre de la lentille.
> * **Axe optique ($\Delta$)** : Axe imaginaire passant perpendiculairement par le centre de la lentille. Il est toujours orienté dans le sens de propagation de la lumière.
> * **Valeur algébrique** : En optique, les distances sont données avec un signe (positif dans le sens de l'axe, négatif dans le sens inverse). On la note avec une barre au-dessus : $\overline{AB}$.

> [!abstract] Foyers et Distance focale
> * **Foyer image ($F'$)** : Point de l'axe optique où converge un faisceau de rayons incidents parallèles à l'axe.
> * **Foyer objet ($F$)** : Point symétrique de $F'$ par rapport au centre optique $O$.
> * **Distance focale ($f'$)** : Distance algébrique entre le centre optique et le foyer image : $f' = \overline{OF'}$. Pour une lentille convergente, $f' > 0$.
> ![Foyers et Distance focale d'une lentille convergente](https://www.schoolmouv.fr/_next/image?url=https%3A%2F%2Fimages.schoolmouv.fr%2Fphysique-chimie-1res-cours01-img12.png&w=1920&q=75)


### 2. Vergence et Rayons principaux

> [!formula] La vergence ($C$)
> La vergence est l'inverse de la distance focale. Plus elle est grande, plus la lentille est "forte" (elle fait converger les rayons plus près).
> $$C = \frac{1}{f'}$$
> * $C$ en dioptries ($\delta$)
> * $f'$ en mètres ($\text{m}$)

> [!tip] Méthode : Les 3 rayons principaux
> Pour trouver l'image $A'B'$ d'un objet $AB$, on trace les rayons issus du point $B$ :
> 1.  Le rayon passant par le centre optique $O$ **n'est pas dévié**.
> 2.  Le rayon incident parallèle à l'axe optique émerge en **passant par le foyer image $F'$**.
> 3.  Le rayon incident passant par le foyer objet $F$ émerge **parallèlement à l'axe optique**.
> ![Tracé des 3 rayons principaux](https://imgs.search.brave.com/c0ELcEwGNt9L2v5ArM-2s2ahaLCgpAE78yNNP1L71gk/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly93d3cu/bWV0aG9kZXBoeXNp/cXVlLmZyL2NvbnN0/cnVjdGlvbl9pbWFn/ZV9sZW50aWxsZS5q/cGc)


---

## II - La Lunette Astronomique

### 1. Principe et Modélisation

> [!info] Constitution
> Une lunette astronomique est un système optique constitué de deux lentilles convergentes :
> * **L'objectif ($L_1$)** : Grande distance focale ($f'_1$). Tourné vers l'objet observé, il collecte la lumière.
> * **L'oculaire ($L_2$)** : Courte distance focale ($f'_2$). Placé près de l'œil, il joue le rôle de loupe.

> [!important] Système Afocal
> Une lunette est réglée pour être **afocale**. Cela signifie qu'elle donne d'un objet situé à l'infini une image rejetée à l'infini (l'œil n'a pas besoin d'accommoder pour l'observer, ce qui évite la fatigue visuelle).
> *Condition* : Pour qu'une lunette soit afocale, le foyer image de l'objectif ($F'_1$) doit être **confondu** avec le foyer objet de l'oculaire ($F_2$).
> La distance entre les deux lentilles vaut donc : $O_1O_2 = f'_1 + f'_2$.


### 2. Tracé des rayons et Formation de l'image

1.  L'objet observé (ex: un cratère lunaire) est à l'infini. Les rayons qui en sont issus arrivent donc **parallèles entre eux** sur l'objectif.
2.  L'objectif forme une **image intermédiaire ($A_1B_1$)** renversée dans son plan focal image (donc en $F'_1$).
3.  Comme le système est afocal ($F'_1$ et $F_2$ sont au même endroit), l'image intermédiaire $A_1B_1$ se trouve exactement dans le plan focal objet de l'oculaire.
4.  L'oculaire agit comme une loupe sur $A_1B_1$ et forme l'**image définitive ($A'B'$) à l'infini**. Les rayons émergent de la lunette parallèles entre eux vers l'œil.
	![Schéma complet de la lunette astronomique afocale|661](https://media-image.kartable.fr/uploads/finalImages/final_5efb58f1647408.89640724.png?format=webp)


### 3. Le Grossissement ($G$)

> [!abstract] Définition
> Le grossissement $G$ (sans unité) est le rapport entre l'angle sous lequel on voit l'image à travers l'instrument ($\theta'$) et l'angle sous lequel on voit l'objet à l'œil nu ($\theta$).
> $$G = \frac{\theta'}{\theta}$$

**Démonstration exigible :**
On se place dans les triangles rectangles formés par les rayons avec l'axe optique. En optique, on utilise l'approximation des petits angles (en radians, $\tan(\alpha) \approx \alpha$) :
* Dans l'objectif : $\tan(\theta) \approx \theta = \frac{A_1B_1}{f'_1}$
* Dans l'oculaire : $\tan(\theta') \approx \theta' = \frac{A_1B_1}{f'_2}$

On remplace dans la formule du grossissement :
$$G = \frac{\frac{A_1B_1}{f'_2}}{\frac{A_1B_1}{f'_1}} = \frac{A_1B_1}{f'_2} \times \frac{f'_1}{A_1B_1}$$

> [!formula] Formule du grossissement de la lunette afocale
> $$G = \frac{f'_1}{f'_2}$$
> *(Pour avoir un fort grossissement, il faut un objectif avec une très grande focale, et un oculaire avec une toute petite focale).*

> [!tip] En pratique
> Il y a souvent plusieurs oculaires vendus avec une lunette, ce qui permet de changer le grossissement. Les caractéristiques commerciales sont données sous la forme "Diamètre / Focale de l'objectif".