# Chapitre 3 : Titrages
**Thème** : [[Constitution et transformations de la matière]]
**Tags** : #physique_chimie #terminale #cours #dosage #titrage

---

## I - Généralités sur les titrages

> [!abstract] Définition : Titrage
> Un titrage est une méthode de dosage s'appuyant sur une **réaction chimique**.

> [!check] Caractéristiques de la réaction support
> Pour qu'une réaction puisse servir de support à un titrage, elle doit obligatoirement être :
> * **Totale** (la réaction va jusqu'à son terme, avancement maximal).
> * **Rapide** (l'état final est atteint quasi instantanément).
> * **Unique** (aucune autre réaction parasite ne doit se produire simultanément).

Soit la réaction support de titrage suivante :
$$aA + bB \rightarrow cC + dD$$

* **Solution titrée (inconnue)** : C'est la solution contenant le réactif $A$ dont on cherche à déterminer la concentration ou la quantité de matière. Elle est placée dans le bécher.
* **Solution titrante (connue)** : C'est la solution contenant le réactif $B$ de concentration connue. Elle est placée dans la burette graduée.

> [!info] Le montage de titrage
> * **En haut** : Potence, burette graduée contenant la solution titrante.
> * **En bas** : Bécher contenant la solution titrée (avec souvent un barreau aimanté), posé sur un agitateur magnétique.
> * **Mesure** : Un appareil de mesure plonge dans le bécher (sonde pH-métrique, cellule conductimétrique...).

---

## II - L'équivalence

### 1. Définition et relation

> [!abstract] Définition : L'équivalence
> On appelle **équivalence** d'un titrage le moment où les réactifs titrant et titré ont été introduits dans les **proportions stœchiométriques** de l'équation de la réaction.
> 
> À l'équivalence, tous les réactifs sont **limitants** (ils sont entièrement consommés).

À partir du tableau d'avancement, si on note $n_A$ la quantité de matière initiale du réactif titré et $n_B$ la quantité de matière de réactif titrant versé à l'équivalence, on obtient :
$n_A - a \cdot x_{max} = 0 \quad \text{et} \quad n_B - b \cdot x_{max} = 0$

> [!formula] Relation à l'équivalence
> À l'équivalence, les quantités de matière vérifient la relation :
> $$\frac{n_A}{a} = \frac{n_B}{b}$$

**Évolution des réactifs au cours du titrage :**
* **Avant l'équivalence** : Le réactif versé (titrant $B$) est le réactif limitant.
* **Après l'équivalence** : Le réactif initial (titré $A$) est entièrement consommé, il est le réactif limitant. Le réactif $B$ s'accumule dans le bécher.

### 2. Complément : Préparation d'une solution (Manuel)
Souvent, on doit déterminer la concentration d'une solution commerciale à l'aide de sa densité $d$ et de son titre massique $P_m$ (en pourcentage).

> [!formula] Formules utiles
> * **Densité** : $d = \frac{\rho_{solution}}{\rho_{eau}}$
> * **Titre massique** : $P_m = \frac{m_{solute}}{m_{solution}}$
> * **Concentration massique** : $C_m = d \times \rho_{eau} \times P_m$
> * **Concentration molaire** : $C = \frac{C_m}{M}$ *(avec $M$ la masse molaire du soluté)*

---

## III - Déterminer l'équivalence

L'objectif pratique d'un titrage est de repérer le volume équivalent $V_{eq}$ (volume de solution titrante versé pour atteindre l'équivalence).

### 1. Titrage pH-métrique
**Condition** : La réaction support est une réaction acido-basique.
**Principe** : On mesure l'évolution du pH au cours de l'ajout de la solution titrante. La courbe $pH = f(V_{versé})$ présente un **saut de pH** brutal à l'équivalence.

> [!tip] Méthode 1 : Méthode des tangentes (Graphique)
> 1. Tracer une première tangente à la courbe avant le saut de pH.
> 2. Tracer une seconde tangente parallèle à la première, après le saut de pH.
> 3. Tracer une droite perpendiculaire à ces deux tangentes.
> 4. Tracer la médiatrice du segment formé (la droite parallèle équidistante aux deux tangentes).
> 5. Le point d'intersection entre cette médiatrice et la courbe correspond au point équivalent. Son abscisse est $V_{eq}$.

> [!tip] Méthode 2 : Méthode de la dérivée (Numérique/Informatique)
> On trace la courbe de la dérivée du pH par rapport au volume : $\frac{dpH}{dV} = f'(V)$.
> L'équivalence est repérée par l'extremum (le **pic**) de cette courbe dérivée. L'abscisse de ce pic correspond à $V_{eq}$.

### 2. Titrage conductimétrique
**Condition** : La réaction support fait intervenir des ions (qui conduisent le courant).
**Principe** : On mesure l'évolution de la conductivité $\sigma$ de la solution. La courbe $\sigma = f(V_{versé})$ est constituée de deux segments de droites. L'équivalence est repérée par la **rupture de pente**. Le point d'intersection des deux segments donne $V_{eq}$.

**Justification de l'allure de la courbe (Loi de Kohlrausch) :**
$$\sigma = \sum \lambda_i \cdot [X_i]$$
L'évolution de la pente s'explique par le remplacement d'un ion par un autre. 
*Exemple générique :*
* **Avant l'équivalence** : Les ions du réactif titré sont consommés, la conductivité peut diminuer ou augmenter selon les conductivités molaires ioniques ($\lambda$) des espèces créées/consommées.
* **Après l'équivalence** : Le réactif titré est épuisé. Les ions de la solution titrante s'accumulent dans le bécher : la conductivité augmente fortement.

### 3. Titrage colorimétrique (Manuel)
**Principe** : L'équivalence est repérée par un **changement de couleur** persistant du milieu réactionnel.
Ce changement de couleur peut être dû à :
* L'un des réactifs ou produits qui est coloré (ex: le diiode ou les ions permanganate).
* L'ajout préalable d'un **indicateur coloré** de fin de réaction (dont la zone de virage doit idéalement encadrer le pH à l'équivalence dans le cas d'un titrage acido-basique).