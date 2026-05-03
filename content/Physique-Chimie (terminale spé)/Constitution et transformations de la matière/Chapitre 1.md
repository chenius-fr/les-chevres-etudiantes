# Chapitre 1 : Les dosages par étalonnage
**Thème** : [[Constitution et transformations de la matière]]
**Tags** : #physique_chimie #terminale #cours #dosage #chimie

---

## Introduction : Rappels de mathématiques

### Fonctions affines et linéaires

> [!abstract] Définition : Fonction affine
> Une fonction est dite affine si elle est de la forme :
> $$f(x) = ax + b \quad \text{avec } a \text{ et } b \in \mathbb{R}^*$$
> **Propriété** : Sa représentation graphique est une droite coupant l'axe des ordonnées à $y = b$.

> [!abstract] Définition : Fonction linéaire
> Une fonction est dite linéaire si elle est de la forme :
> $$f(x) = ax$$
> **Propriété** : Sa représentation graphique est une droite passant par l'origine du repère.

* **Remarque 1** : Si une représentation graphique est une droite passant par l'origine $O$, on a alors $y = ax$, et on dit que $y$ est proportionnel à $x$.
* **Remarque 2** : Si $y$ est proportionnel à $x$, alors sa représentation graphique est une droite passant par $O$.

### Le coefficient directeur

> [!formula] Propriété : Calcul du coefficient directeur
> Le coefficient directeur $a$ d'une droite est donné par :
> $$a = \frac{\Delta y}{\Delta x} = \frac{y_B - y_A}{x_B - x_A}$$
> *avec $A$ et $B$, deux points de la courbe.*

> [!tip] Conseil
> Si c'est une fonction linéaire, prendre l'origine $O(0,0)$ pour l'un des points. Sinon, prendre des points sur les axes si possible pour faciliter la lecture.

---

## 1. Principe d'un dosage

### 1.1. Généralités
Le but d'un dosage est de déterminer la **concentration d'une solution**.

> [!info] Principe du dosage par étalonnage
> Il consiste à utiliser une gamme étalon de solutions de concentrations connues pour déterminer la concentration d'une solution inconnue.

Pour comparer les solutions, on va mesurer une grandeur physique :
* L'absorbance $A$ (sans unité)
* La conductivité $\sigma$ (en $\text{S}\cdot\text{cm}^{-1}$ ou $\text{S}\cdot\text{m}^{-1}$)
* La densité (plus difficile à mettre en œuvre)

### 1.2. Point méthode : La dilution
Pour réaliser la gamme étalon, on utilise la méthode des dilutions.

> [!formula] Propriété fondamentale de la dilution
> Lors d'une dilution, la quantité de matière de soluté ne change pas :
> $$n_i = n_f$$
> Or, comme $n = C \times V$, on en déduit :
> $$C_i \times V_i = C_f \times V_f$$
> Soit, avec les notations mère/fille :
> $$C_m \times V_m = C_f \times V_f$$

> [!warning] À SAVOIR (Matériel)
> * $V_m$ (volume de la solution mère à prélever) est mesuré à l'aide d'une **pipette jaugée**.
> * $V_f$ (volume de la solution fille à préparer) est mesuré à l'aide d'une **fiole jaugée**.
> * Toujours vérifier que : $V_f > V_m$ et $C_m > C_f$.

### 1.3. Le facteur de dilution

> [!formula] Définition : Facteur de dilution
> Le facteur de dilution, parfois noté $n$ (ou $F$), est donné par :
> $$n = \frac{C_m}{C_f}$$
> D'après la formule de dilution ($C_m \cdot V_m = C_f \cdot V_f$), on a aussi :
> $$n = \frac{V_f}{V_m}$$

> [!example] Exemple d'application
> Si je dois préparer $100 \text{ mL}$ d'une solution diluée $5 \text{ fois}$ :
> * $V_f = 100 \text{ mL}$ et $n = 5$
> * Donc le volume à prélever est : $V_m = \frac{V_f}{n} = \frac{100}{5} = 20 \text{ mL}$

---

## 2. Les types de dosages par étalonnage

### 2.1. Le dosage colorimétrique
Dans ce cas, on mesure l'absorbance des solutions de la gamme étalon et on trace le graphique d'étalonnage : $A = f(C)$.

> [!formula] Loi de Beer-Lambert
> L'absorbance d'une solution est proportionnelle à sa concentration :
> $$A = k \cdot C$$

* **Remarque graphique** : D'après la loi de Beer-Lambert, la courbe obtenue est une droite passant par l'origine $O$.
* **Détermination** : Pour déterminer la concentration de notre solution inconnue, on mesure son absorbance et on lit directement sa concentration sur le graphique par report.
* **Paramétrage** : L'absorbance des solutions est mesurée à la longueur d'onde donnant le maximum d'absorbance ($\lambda_{max}$).

### 2.2. Le dosage conductimétrique
Le principe est identique au dosage colorimétrique (point 2.1), mais on remplace l'absorbance $A$ par la conductivité $\sigma$, et la loi de Beer-Lambert par la loi de Kohlrausch.

> [!formula] Loi de Kohlrausch
> La conductivité $\sigma$ (souvent en $\text{S}\cdot\text{m}^{-1}$) d'une solution ionique diluée est proportionnelle à la concentration des ions présents :
> $$\sigma = \sum \lambda_i \cdot C_i$$
> * $\lambda_i$ : conductivité molaire ionique de l'espèce $i$
> * $C_i$ : concentration de l'espèce $i$