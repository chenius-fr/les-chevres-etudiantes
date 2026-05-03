# Chapitre 4 : Mécanique Newtonienne
**Thème** : [[Mouvement et interactions]]
**Tags** : #physique_chimie #terminale #cours #mécanique #newton #cinématique

---

## I - Rappels mathématiques et physiques

### 1. Points Maths : Trigonométrie et Dérivation

> [!tip] Trigonométrie dans le triangle rectangle
> Pour un angle $\alpha$ dans un triangle rectangle (côtés $a, b$, hypoténuse $c$) :
> * **Pythagore** : $c = \sqrt{a^2 + b^2}$
> * **SOH-CAH-TOA** : $\sin(\alpha) = \frac{\text{Opposé}}{\text{Hypoténuse}}$, $\cos(\alpha) = \frac{\text{Adjacent}}{\text{Hypoténuse}}$, $\tan(\alpha) = \frac{\text{Opposé}}{\text{Adjacent}}$

> [!formula] Dérivées et Primitives usuelles
> La dérivée $f'(x)$ donne les variations de $f(x)$.
> *En mathématiques :* $f(x) = x^n \implies f'(x) = n x^{n-1}$
> *En physique (selon le temps $t$) :* $f'(t) \Leftrightarrow \frac{df}{dt}$ et $\frac{d}{dt}(t^n) = n t^{n-1}$
> 
> **Définition :** Une primitive $F(x)$ est une fonction telle que $F'(x) = f(x)$.
> 
> | Fonction $f(t)$ | Primitive $F(t)$ |
> | :--- | :--- |
> | $0$ | $C \in \mathbb{R}$ (constante) |
> | $1$ | $t + C$ |
> | $k$ (constante) | $k \cdot t + C$ |
> | $k \cdot t$ | $\frac{k \cdot t^2}{2} + C$ |
> | $k \cdot t^n$ | $k \cdot \frac{t^{n+1}}{n+1} + C$ |

### 2. Points Physiques : Référentiels et Forces

> [!info] Définitions
> * **Référentiel** : Objet ou point de l'espace qui sert de référence au mouvement. Les 3 principaux sont :
>   * *Héliocentrique* (centre du Soleil)
>   * *Géocentrique* (centre de la Terre)
>   * *Terrestre* (laboratoire = point à la surface de la Terre)
> * **Force ($\vec{F}$)** : Représentée par un vecteur (norme, direction, sens), c'est une interaction qui influence le mouvement. Son intensité $F$ s'exprime en Newton (N).

---

## II - Dynamique Newtonienne : Les lois de Newton

> [!abstract] 1ère Loi de Newton : Principe d'inertie
> Un corps soumis à des forces qui se compensent ($\sum \vec{F}_{ext} = \vec{0}$) est soit animé d'un mouvement rectiligne uniforme (vitesse constante), soit au repos.

> [!important] 2ème Loi de Newton : Principe Fondamental de la Dynamique (PFD)
> Dans un référentiel galiléen, la masse $m$ d'un corps multipliée par l'accélération de son centre de masse $\vec{a}$ est égale à la somme vectorielle des forces extérieures qui s'y appliquent :
> $$m \cdot \vec{a} = \sum \vec{F}_{ext}$$

> [!abstract] 3ème Loi de Newton : Principe des actions réciproques
> Un corps A exerçant sur un corps B une force $\vec{F}_{A/B}$ subit en retour une force $\vec{F}_{B/A}$ de même intensité, de même direction, mais de sens opposé :
> $$\vec{F}_{A/B} = -\vec{F}_{B/A}$$

---

## III - Application 1 : Chute libre sans vitesse initiale

> [!info] Définition : Chute libre
> Un système est en chute libre s'il n'est soumis qu'à l'action de son poids $\vec{P}$. 
> *Situation : Considérons un corps de masse $m$ lâché d'une hauteur $h$ dans un champ de pesanteur, sans vitesse initiale.*

**Méthode de résolution pas-à-pas :**
**1)** Système : corps de masse $m$
**2)** Référentiel : terrestre supposé galiléen
**3)** Repère : $(O; \vec{i}, \vec{j})$
**4)** Bilan des forces : Poids $\vec{P} = m \cdot \vec{g}$
**5)** PFD : D'après la 2ème loi de Newton :
$m \cdot \vec{a} = \sum \vec{F}_{ext} \implies m \cdot \vec{a} = \vec{P} \implies m \cdot \vec{a} = m \cdot \vec{g} \implies \vec{a} = \vec{g}$
*(Le mouvement d'un corps en chute libre ne dépend pas de sa masse).*

**6)** Exprimons les coordonnées : $\vec{a} \begin{pmatrix} a_x \\ a_y \end{pmatrix}$ et $\vec{g} \begin{pmatrix} 0 \\ -g \end{pmatrix} \implies \begin{cases} a_x = 0 \\ a_y = -g \end{cases}$
**7)** On a $\vec{a} = \frac{d\vec{v}}{dt}$, on cherche la primitive de $\vec{a}$ pour avoir $\vec{v}$ : $\begin{cases} v_x = C_{x1} \\ v_y = -gt + C_{y1} \end{cases}$
**8)** Constantes avec les Conditions Initiales (CI) : À $t=0$, l'objet est lâché sans vitesse initiale, donc $\begin{cases} v_{x0} = 0 \\ v_{y0} = 0 \end{cases}$
**9)** Cas général (la vitesse) : $\begin{cases} v_x = 0 \\ v_y = -gt \end{cases}$
**10)** On a $\vec{v} = \frac{d\vec{OG}}{dt}$, on cherche la primitive de $\vec{v}$ pour avoir la position $\vec{OG}$ : $\begin{cases} x = C_{x2} \\ y = -\frac{1}{2}gt^2 + C_{y2} \end{cases}$
**11)** Constantes avec les CI : À $t=0$, l'objet est à la hauteur $h$, donc $\begin{cases} x_0 = 0 \\ y_0 = h \end{cases}$
**12)** Cas général (la position) : $\begin{cases} x = 0 \\ y = -\frac{1}{2}gt^2 + h \end{cases}$

*(Note : Les équations de $\vec{a}$, $\vec{v}$ et $\vec{OG}$ en fonction du temps sont appelées les **équations horaires** du mouvement).*

---

## IV - Application 2 : Chute libre avec vitesse initiale

*Situation : Un objet de masse $m$ est lancé d'une hauteur $h$ avec une vitesse initiale $\vec{v}_0$ faisant un angle $\alpha$ avec l'axe (Ox).*

Les étapes **1 à 5** sont identiques. On a donc l'accélération : $\vec{a} = \vec{g}$.
**6)** Coordonnées de l'accélération : $\begin{cases} a_x = 0 \\ a_y = -g \end{cases}$
**7)** Primitive pour la vitesse : $\begin{cases} v_x = C_{x1} \\ v_y = -gt + C_{y1} \end{cases}$
**8)** Constantes avec les CI : À $t=0$, le vecteur $\vec{v}_0$ est incliné d'un angle $\alpha$. Par trigonométrie : $\begin{cases} v_{x0} = v_0 \cdot \cos(\alpha) \\ v_{y0} = v_0 \cdot \sin(\alpha) \end{cases}$
**9)** Cas général (la vitesse) : $\begin{cases} v_x = v_0 \cdot \cos(\alpha) \\ v_y = -gt + v_0 \cdot \sin(\alpha) \end{cases}$
**10)** Primitive pour la position $\vec{OG}$ : $\begin{cases} x = (v_0 \cdot \cos(\alpha)) \cdot t + C_{x2} \\ y = -\frac{1}{2}gt^2 + (v_0 \cdot \sin(\alpha)) \cdot t + C_{y2} \end{cases}$
**11)** Constantes avec les CI : À $t=0$, $\begin{cases} x_0 = 0 \\ y_0 = h \end{cases}$
**12)** Cas général (la position) : $\begin{cases} x = (v_0 \cdot \cos(\alpha)) \cdot t \\ y = -\frac{1}{2}gt^2 + (v_0 \cdot \sin(\alpha)) \cdot t + h \end{cases}$

**13)** L'équation de la trajectoire (élimination du paramètre temps $t$) :
D'après l'équation de $x$, on a $t = \frac{x}{v_0 \cdot \cos(\alpha)}$. On remplace $t$ dans l'équation de $y$ :
$$y = -\frac{1}{2}g \left(\frac{x}{v_0 \cdot \cos(\alpha)}\right)^2 + v_0 \cdot \sin(\alpha) \left(\frac{x}{v_0 \cdot \cos(\alpha)}\right) + h$$

> [!formula] Équation de la trajectoire (Parabole)
> $$y = -\frac{g}{2 \cdot v_0^2 \cdot \cos^2(\alpha)} \cdot x^2 + \tan(\alpha) \cdot x + h$$

---

## V - Application 3 : Particule chargée dans un condensateur plan

### 1. Rappels sur le condensateur
> [!info] Le condensateur plan
> Un condensateur plan est constitué de 2 plaques métalliques séparées par un isolant. S'il est alimenté par une tension $U$, il génère entre ses plaques espacées d'une distance $d$ un **champ électrique uniforme $\vec{E}$** dirigé du $+$ vers le $-$.
> Son intensité est : $E = \frac{U}{d}$ (en $\text{V}\cdot\text{m}^{-1}$)

> [!abstract] Force électrique
> Une particule de charge $q$ dans un champ $\vec{E}$ subit une force électrique $\vec{F}_E$ telle que :
> $$\vec{F}_E = q \cdot \vec{E}$$

### 2. Mouvement d'une particule
*Situation : Une particule de masse $m$ et de charge $q$ est lancée avec une vitesse horizontale $\vec{v}_0$ entre les plaques d'un condensateur où règne un champ $\vec{E}$ vertical.*

**1 à 4)** Système (particule), Référentiel (terrestre), Repère $(O; \vec{i}, \vec{j})$. Bilan des forces : $\vec{F}_E = q \cdot \vec{E}$ (Le poids $\vec{P}$ est négligé devant la force électrique).
**5)** PFD : $m \cdot \vec{a} = \sum \vec{F}_{ext} \implies m \cdot \vec{a} = q \cdot \vec{E} \implies \vec{a} = \frac{q}{m}\vec{E}$
**6)** Coordonnées : $\vec{a} \begin{pmatrix} a_x \\ a_y \end{pmatrix} = \frac{q}{m} \begin{pmatrix} 0 \\ E \end{pmatrix} \implies \begin{cases} a_x = 0 \\ a_y = \frac{q \cdot E}{m} \end{cases}$
**7)** Primitive (vitesse) : $\begin{cases} v_x = C_{x1} \\ v_y = \frac{q \cdot E}{m}t + C_{y1} \end{cases}$
**8)** Constantes (CI) : Vitesse initiale horizontale, donc $\begin{cases} v_{x0} = v_0 \\ v_{y0} = 0 \end{cases}$
**9)** Cas général (vitesse) : $\begin{cases} v_x = v_0 \\ v_y = \frac{q \cdot E}{m}t \end{cases}$
**10)** Primitive (position) : $\begin{cases} x = v_0 \cdot t + C_{x2} \\ y = \frac{q \cdot E}{2m}t^2 + C_{y2} \end{cases}$
**11)** Constantes (CI) : Départ à l'origine, donc $\begin{cases} x_0 = 0 \\ y_0 = 0 \end{cases}$
**12)** Cas général (position) : $\begin{cases} x = v_0 \cdot t \\ y = \frac{q \cdot E}{2m}t^2 \end{cases}$

**13)** Équation de la trajectoire :
On isole $t = \frac{x}{v_0}$ et on remplace dans $y$ :

> [!formula] Équation de la trajectoire (Particule chargée)
> $$y = \frac{q \cdot E}{2 \cdot m \cdot v_0^2} \cdot x^2$$