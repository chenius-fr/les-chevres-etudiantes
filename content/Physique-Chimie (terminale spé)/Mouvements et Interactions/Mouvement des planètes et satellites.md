---
title: Mouvement des planètes et satellites
tags:
  - physique_chimie
  - terminale
  - cours
  - mécanique
  - kepler
  - astrophysique
---

**Thème** : [[Mouvement et interactions]]

---

## I - Formalisme et outils mathématiques

### 1. La gravitation universelle

> [!abstract] Définition : Force de gravitation universelle
> La gravitation universelle est une interaction attractive de portée infinie entre deux corps possédant une masse.
> Soit deux corps $A$ et $B$ de masses respectives $m_A$ et $m_B$, séparés d'une distance $d$. La force exercée par $A$ sur $B$ s'écrit :
> 
> $$\vec{F}_{A/B} = - G \frac{m_A \cdot m_B}{d^2} \vec{u}_{AB}$$
> 
> * $\vec{u}_{AB}$ : vecteur unitaire dirigé de $A$ vers $B$.
> * $G$ : constante de gravitation universelle ($G \simeq 6,67 \times 10^{-11} \text{ N}\cdot\text{m}^2\cdot\text{kg}^{-2}$).

> [!info] Lien avec le Poids (Cas particulier)
> Le poids $\vec{P}$ d'un objet correspond à la force de gravitation universelle exercée par la Terre sur cet objet à sa surface.
> Pour un objet de masse $m$ à la surface de la Terre :
> $$F_G = G \frac{m \cdot M_T}{R_T^2} \implies P = m \cdot g \quad \text{avec} \quad g = \frac{G \cdot M_T}{R_T^2} \simeq 9,8 \text{ m}\cdot\text{s}^{-2}$$

### 2. Le repère de Frenet
Pour étudier un mouvement courbe ou circulaire, il est plus simple d'utiliser le repère de Frenet plutôt que le repère cartésien $(O; \vec{i}, \vec{j})$.

> [!formula] Accélération dans le repère de Frenet
> Le repère de Frenet est lié au centre de masse de l'objet en mouvement. Il est défini par deux vecteurs unitaires :
> * $\vec{u}_T$ : vecteur tangent à la trajectoire, dans le sens du mouvement.
> * $\vec{u}_N$ : vecteur normal, orthogonal à $\vec{u}_T$ et dirigé vers le centre de la courbure.
> 
> Pour une **orbite circulaire** de rayon $r$, le vecteur accélération s'écrit :
> $$\vec{a} \begin{pmatrix} a_N = \frac{v^2}{r} \\ a_T = \frac{dv}{dt} \end{pmatrix}$$

---

## II - Étude dynamique : Mouvement d'une planète

*Situation : Étude du mouvement de la Terre (masse $M_T$) autour du Soleil (masse $M_S$) sur une orbite supposée circulaire de rayon $r$.*

**Application du Principe Fondamental de la Dynamique (PFD) :**
**1)** **Système** : La Terre de masse $M_T$
**2)** **Référentiel** : Héliocentrique (supposé galiléen)
**3)** **Repère** : Repère de Frenet $(\vec{u}_T, \vec{u}_N)$
**4)** **Bilan des forces** : Force de gravitation exercée par le Soleil sur la Terre : $\vec{F}_G = G \frac{M_T \cdot M_S}{r^2} \vec{u}_N$
**5)** **2ème loi de Newton** : 
$$M_T \cdot \vec{a} = \sum \vec{F}_{ext} \implies M_T \cdot \vec{a} = G \frac{M_T \cdot M_S}{r^2} \vec{u}_N \implies \vec{a} = G \frac{M_S}{r^2} \vec{u}_N$$
**6)** **Coordonnées de l'accélération** (en identifiant avec les formules de Frenet) :
$$\begin{cases} a_N = \frac{v^2}{r} = G \frac{M_S}{r^2} \\ a_T = \frac{dv}{dt} = 0 \end{cases}$$

### 1. Nature du mouvement
D'après l'étape 6, on a $a_T = \frac{dv}{dt} = 0$.
Donc la vitesse $v$ est **constante**. Le mouvement de la Terre est **circulaire et uniforme**.
> [!warning] Attention
> La valeur (norme) de la vitesse ne change pas, mais la direction du vecteur vitesse $\vec{v}$ change à chaque instant puisqu'il suit la courbe de l'orbite !

### 2. Expression de la vitesse orbitale ($v$)
D'après l'équation sur l'axe normal ($\vec{u}_N$) :
$$\frac{v^2}{r} = G \frac{M_S}{r^2} \implies v^2 = G \frac{M_S}{r}$$
$$v = \sqrt{\frac{G \cdot M_S}{r}}$$

### 3. Période de révolution ($T$)
> [!abstract] Définition : Période de révolution
> La période de révolution $T$ est la durée nécessaire pour que la planète fasse un tour complet sur son orbite.

La distance parcourue pour un tour est le périmètre du cercle : $d = 2\pi r$.
Comme la vitesse est constante, $v = \frac{d}{T} = \frac{2\pi r}{T} \implies T = \frac{2\pi r}{v}$.
En remplaçant $v$ par son expression :
$$T = \frac{2\pi r}{\sqrt{\frac{G \cdot M_S}{r}}} \implies T = 2\pi \sqrt{\frac{r^3}{G \cdot M_S}}$$

---

## III - Les lois de Kepler

Ces lois, initialement formulées pour les planètes autour du Soleil, se généralisent à tout satellite en orbite autour d'un astre attracteur (ex: la Lune ou un satellite artificiel autour de la Terre).

> [!abstract] 1ère loi de Kepler : Loi des orbites
> Dans le référentiel héliocentrique, la trajectoire du centre de masse d'une planète est une **ellipse** dont le Soleil est l'un des foyers.
> *(Remarque : Le cercle est une ellipse particulière où les deux foyers sont confondus au centre).*

> [!abstract] 2ème loi de Kepler : Loi des aires
> Le segment de droite reliant le centre du Soleil et le centre de la planète balaie des **aires égales** pendant des **durées égales**.
> *(Conséquence : La planète se déplace plus vite lorsqu'elle est proche du Soleil, et plus lentement lorsqu'elle en est éloignée).*

> [!formula] 3ème loi de Kepler : Loi des périodes
> Pour toutes les planètes du système solaire, le rapport entre le carré de la période de révolution $T$ et le cube du demi-grand axe $a$ de l'ellipse est constant.
> $$\frac{T^2}{a^3} = \text{constante}$$
> 
> *Démonstration dans le cas d'une orbite circulaire de rayon $r$ (où $a = r$) :*
> On a vu que $T = 2\pi \sqrt{\frac{r^3}{G \cdot M_S}}$. En élevant au carré :
> $$T^2 = \frac{4\pi^2 \cdot r^3}{G \cdot M_S} \implies \frac{T^2}{r^3} = \frac{4\pi^2}{G \cdot M_S}$$
> La constante ne dépend que de la masse de l'astre attracteur central ($M_S$).

---

## IV - Complément : Le satellite géostationnaire

> [!info] Propriétés d'un satellite géostationnaire
> Un satellite artificiel est dit géostationnaire s'il paraît **immobile** pour un observateur terrestre. Pour cela, il doit respecter 3 conditions strictes :
> 1. Son orbite doit être dans le **plan de l'équateur**.
> 2. Il doit tourner dans le **même sens** que la Terre.
> 3. Sa période de révolution doit être exactement égale à la période de rotation propre de la Terre ($T \simeq 24\text{h}$ ou $86164\text{ s}$).
> 
> *Conséquence* : Son altitude est unique et fixée à environ **35 800 km**.