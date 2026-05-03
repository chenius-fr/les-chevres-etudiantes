---
title: Transferts thermiques
tags:
  - physique_chimie
  - terminale
  - cours
  - thermodynamique
  - énergie
---

**Thème** : [[L'énergie : conversions et transferts]]

---

## Introduction : Les Gaz Parfaits

> [!formula] Équation d'état des gaz parfaits
> Un gaz parfait est un modèle thermodynamique où l'on néglige les interactions entre les molécules.
> $$P \cdot V = n \cdot R \cdot T$$
> * $P$ : Pression du gaz en Pascals (Pa)
> * $V$ : Volume du gaz en mètres cubes ($\text{m}^3$)
> * $n$ : Quantité de matière en moles (mol)
> * $R$ : Constante des gaz parfaits ($R \simeq 8,31 \text{ J}\cdot\text{mol}^{-1}\cdot\text{K}^{-1}$)
> * $T$ : Température absolue en Kelvins (K)

*Remarque* : Pour une quantité de gaz donnée à température constante, on a la loi de Boyle-Mariotte : $P \times V = \text{constante}$.

---

## I - Le Premier Principe de la Thermodynamique

### 1. L'énergie interne ($U$)
L'énergie interne $U$ (en Joules) d'un système correspond à la somme des énergies cinétiques microscopiques (agitation thermique) et des énergies potentielles d'interaction entre les particules du système.
*Propriété* : L'énergie interne d'un système ne dépend que de sa température $T$.

> [!important] Le Premier Principe
> Au cours d'une transformation, la variation d'énergie interne $\Delta U$ d'un système fermé est égale à la somme du travail mécanique $W$ et du transfert thermique $Q$ échangés avec le milieu extérieur.
> $$\Delta U = W + Q$$
> *(Conventions de signe : $W$ et $Q$ sont comptés $> 0$ s'ils sont reçus par le système, et $< 0$ s'ils sont cédés par le système au milieu extérieur).*

### 2. Cas du système incompressible
> [!info] Définition
> Un système est dit incompressible si son volume ne varie pas (c'est le cas des solides et des liquides). Le travail des forces de pression est alors nul ($W = 0$).

> [!formula] Variation d'énergie interne (Solide/Liquide)
> Pour un système incompressible de masse $m$ n'échangeant pas de travail :
> $$\Delta U = Q = m \cdot c \cdot \Delta T$$
> Soit : $\Delta U = m \cdot c \cdot (T_f - T_i)$
> * $c$ : Capacité thermique massique en $\text{J}\cdot\text{kg}^{-1}\cdot\text{K}^{-1}$ (ou $\text{J}\cdot\text{kg}^{-1}\cdot^\circ\text{C}^{-1}$)
> * $\Delta T$ : Variation de température. Comme $T(\text{K}) = \theta(^\circ\text{C}) + 273,15$, un écart de température est identique dans les deux unités : $\Delta T = \Delta \theta$.

---

## II - Modes et Transferts Thermiques

**Règle fondamentale** : Un transfert thermique (la chaleur) s'effectue toujours spontanément du corps le plus chaud vers le corps le plus froid.

### 1. Les 3 modes de transfert
1. **La conduction** : Transfert d'énergie de proche en proche, **sans** déplacement global de matière. C'est le mode principal dans les solides.
2. **La convection** : Transfert d'énergie **avec** déplacement macroscopique de matière. C'est le mode propre aux fluides (liquides et gaz). Les courants de fluide chaud montent (moins denses) et les fluides froids descendent.
3. **Le rayonnement** : Transfert d'énergie s'effectuant par l'émission et l'absorption d'ondes électromagnétiques (OEM). Il peut se faire même dans le vide.

### 2. Le Flux Thermique ($\Phi$)
> [!abstract] Définition : Flux thermique
> Le flux thermique $\Phi$ (Phi) est la puissance thermique transférée. C'est l'énergie thermique $Q$ échangée par unité de temps $\Delta t$.
> $$\Phi = \frac{Q}{\Delta t}$$
> * $\Phi$ s'exprime en Watts (W)
> * $Q$ en Joules (J) et $\Delta t$ en secondes (s)

### 3. La Résistance Thermique ($R_{th}$)
Tout comme une résistance électrique s'oppose au passage du courant, une paroi s'oppose au passage du flux thermique.

> [!formula] Loi d'Ohm thermique
> Le flux thermique $\Phi$ à travers une paroi séparant deux milieux aux températures $T_1$ et $T_2$ (avec $T_1 > T_2$) est donné par :
> $$\Phi = \frac{T_1 - T_2}{R_{th}}$$
> * $R_{th}$ : Résistance thermique en $\text{K}\cdot\text{W}^{-1}$ (ou $^\circ\text{C}\cdot\text{W}^{-1}$). Plus $R_{th}$ est grande, plus le matériau est isolant.

---

## III - Bilan Thermique : La Loi de Newton

### 1. La Loi de refroidissement de Newton
Cette loi modélise les échanges par **convection** entre un système (à la température $T$) et l'air environnant ou un thermostat (à la température $T_{ext}$ ou $T_e$).

> [!formula] Flux convectif de Newton
> $$\Phi = h \cdot S \cdot (T_{ext} - T)$$
> * $h$ : Coefficient d'échange convectif en $\text{W}\cdot\text{m}^{-2}\cdot\text{K}^{-1}$
> * $S$ : Surface d'échange en $\text{m}^2$
> *(Si $T < T_{ext}$, le système reçoit de l'énergie, $\Phi > 0$. Si $T > T_{ext}$, le système cède de l'énergie, $\Phi < 0$).*

### 2. L'équation différentielle de l'évolution de la température
Considérons un système incompressible (masse $m$, capacité $c$) qui se refroidit ou se réchauffe au contact d'un thermostat extérieur ($T_{ext}$).

D'après le 1er principe, pour une petite durée $dt$, l'énergie échangée est $dQ = m \cdot c \cdot dT$.
Or, d'après la définition du flux : $dQ = \Phi \cdot dt$.
Donc : $m \cdot c \cdot dT = \Phi \cdot dt \implies m \cdot c \cdot \frac{dT}{dt} = \Phi$

En remplaçant $\Phi$ par l'expression de la loi de Newton :
$$m \cdot c \cdot \frac{dT}{dt} = h \cdot S \cdot (T_{ext} - T)$$
En divisant tout par $m \cdot c$ et en réorganisant, on obtient l'équation différentielle linéaire du 1er ordre :

> [!important] Équation différentielle de la température
> $$\frac{dT}{dt} + \frac{h \cdot S}{m \cdot c} \cdot T = \frac{h \cdot S}{m \cdot c} \cdot T_{ext}$$

### 3. Résolution et Temps caractéristique ($\tau$)
On pose le temps caractéristique du système $\tau = \frac{m \cdot c}{h \cdot S}$ (en secondes).
La solution mathématique de cette équation est de la forme :
$$T(t) = (T_{initial} - T_{ext}) \cdot e^{-\frac{t}{\tau}} + T_{ext}$$

> [!tip] Analogie avec le condensateur (Circuit RC)
> L'évolution de la température suit exactement la même logique exponentielle que la charge ou la décharge d'un condensateur (où $\tau = R \cdot C$). Ici, l'équivalent de la capacité est $m \cdot c$ et l'équivalent de la résistance est $\frac{1}{h \cdot S}$. Le régime permanent est atteint au bout d'environ $5\tau$.

---

## IV - Bilan Radiatif Terrestre (Rayonnement)

### 1. Loi de Stefan-Boltzmann
> [!formula] Puissance rayonnée
> Tout corps chaud émet un rayonnement électromagnétique. La puissance totale rayonnée $P$ (en Watts) par un corps noir (modèle idéal) dépend de sa température absolue :
> $$P = \sigma \cdot S \cdot T^4$$
> * $\sigma$ : Constante de Stefan-Boltzmann ($\simeq 5,67 \times 10^{-8} \text{ W}\cdot\text{m}^{-2}\cdot\text{K}^{-4}$)

### 2. Albédo et Effet de Serre
* **Albédo ($a$ ou $\alpha$)** : Grandeur sans unité comprise entre 0 et 1. C'est le rapport entre la puissance rayonnée diffusée (réfléchie) par une surface et la puissance incidente qu'elle reçoit.
  $$a = \frac{P_{diffusee}}{P_{incidente}}$$
  *(La neige a un fort albédo, l'océan a un faible albédo).*
* **Effet de serre** : L'atmosphère terrestre est transparente au rayonnement visible venant du Soleil, mais elle absorbe en grande partie les rayonnements Infrarouges (IR) réémis par la surface de la Terre. L'atmosphère réémet ensuite cette énergie vers le sol, augmentant ainsi la température moyenne d'équilibre du système.