---
title: Radioactivité
tags:
  - physique_chimie
  - terminale
  - cours
  - nucléaire
  - radioactivité
---

**Thème** : [[Constitution et transformations de la matière]]
**Tags** : #physique_chimie #terminale #cours #nucléaire #radioactivité

---

## Introduction : Le noyau atomique

> [!abstract] Définition : Notation symbolique
> Le noyau d'un atome est constitué de protons (chargés positivement) et de neutrons (neutres), appelés collectivement les **nucléons**.
> La notation symbolique d'un noyau est de la forme :
> $$_{Z}^{A}\text{X}$$
> * **A** : Nombre de masse (nombre total de nucléons).
> * **Z** : Numéro atomique (nombre de protons).
> * **X** : Symbole de l'élément chimique.

> [!important] Loi de conservation (Lois de Soddy)
> Au cours d'une transformation nucléaire, la somme des nombres de masse ($A$) et la somme des numéros atomiques ($Z$) se conservent.

---

## I - Les types de radioactivité

> [!info] Définition : Radioactivité
> La radioactivité est un phénomène physique naturel, aléatoire et spontané. C'est l'ensemble des transformations du noyau instable d'un atome (le noyau "père") qui se désintègre en un autre noyau (le noyau "fils") avec l'émission d'une particule et/ou d'un rayonnement.

### 1. Radioactivité $\alpha$ (Alpha)
* **Cause** : Surplus de nucléons (concerne les noyaux lourds).
* **Particule émise** : Noyau d'Hélium appelées particules $\alpha$ ($_{2}^{4}\text{He}$).
* **Équation de réaction** :
  $$_{Z}^{A}\text{X} \rightarrow _{Z-2}^{A-4}\text{Y} + _{2}^{4}\text{He}$$
* **Dangerosité & Protection** : Très dangereuse car la particule possède une forte énergie cinétique, mais **faible pouvoir pénétrant**. Une simple *feuille de papier* ou la peau suffit à l'arrêter.

### 2. Radioactivité $\beta^-$ (Bêta moins)
* **Cause** : Excès de neutrons (un neutron se transforme en proton).
* **Particule émise** : Un électron ($_{-1}^{0}\text{e}$).
* **Équation de réaction** :
  $$_{Z}^{A}\text{X} \rightarrow _{Z+1}^{A}\text{Y} + _{-1}^{0}\text{e}$$

### 3. Radioactivité $\beta^+$ (Bêta plus)
* **Cause** : Excès de protons (un proton se transforme en neutron).
* **Particule émise** : Un positron ou positon ($_{+1}^{0}\text{e}$, l'antiparticule de l'électron).
* **Équation de réaction** :
  $$_{Z}^{A}\text{X} \rightarrow _{Z-1}^{A}\text{Y} + _{+1}^{0}\text{e}$$

> [!warning] Dangerosité des rayonnements $\beta$
> Les particules $\beta$ ont une dangerosité assez forte (risques de brûlures et de mutations). Leur pouvoir pénétrant est modéré : elles sont arrêtées par une *feuille d'aluminium* ou quelques millimètres de verre.

### 4. Rayonnement $\gamma$ (Gamma)
* **Cause** : Désexcitation du noyau fils après une désintégration $\alpha$ ou $\beta$. Le noyau fils est souvent créé dans un état excité (noté avec un astérisque $Y^*$).
* **Particule émise** : Un photon (onde électromagnétique de très courte longueur d'onde et de très haute énergie).
* **Équation de réaction** :
  $$_{Z}^{A}\text{Y}^{*} \rightarrow _{Z}^{A}\text{Y} + \gamma$$
* **Dangerosité & Protection** : Extrêmement dangereux. **Grand pouvoir pénétrant**, nécessitant d'épaisses couches de protection (*10 cm de plomb ou 1 mètre de béton*).

---

## II - Fission et Fusion nucléaires (Autres transformations)

* **Fission nucléaire** : Un noyau lourd (ex: Uranium 235) se "casse" sous l'impact d'un neutron pour former deux noyaux plus petits et plus stables.
  * *Risque* : Dégage d'autres neutrons qui vont provoquer une réaction en chaîne (risque d'explosion si non contrôlée).
* **Fusion nucléaire** : Deux petits noyaux légers (ex: isotopes de l'hydrogène) s'assemblent pour former un noyau plus lourd.
  * *Condition* : Nécessite une chaleur extrême (se produit naturellement au cœur des étoiles comme le Soleil).

---

## III - La loi de décroissance radioactive

> [!tip] Comportement statistique
> La désintégration d'un seul noyau radioactif se produit **aléatoirement**. Cependant, sur un échantillon contenant un très grand nombre d'atomes, la décroissance évolue de façon **régulière et prévisible**.

### 1. L'équation différentielle (Loi d'ordre 1)
La variation du nombre de noyaux $N(t)$ au cours du temps est proportionnelle au nombre de noyaux présents. C'est une réaction qui suit une **cinétique d'ordre 1**.

> [!formula] Équation différentielle
> $$\frac{dN(t)}{dt} = -\lambda \cdot N(t)$$
> * $\lambda$ (lambda) : **constante radioactive** de l'élément (en $\text{s}^{-1}$, $\text{h}^{-1}$ ou $\text{an}^{-1}$).

> [!tip] Point Math : Résolution
> L'équation différentielle du premier ordre $y' = ay + b$ a pour solution $y = K e^{ax} - \frac{b}{a}$.
> Ici, $a = -\lambda$ et $b = 0$. On obtient donc directement la solution :

> [!formula] Loi de décroissance
> Le nombre de noyaux radioactifs restants à l'instant $t$ est modélisé par :
> $$N(t) = N_0 \cdot \exp(-\lambda \cdot t)$$
> * $N_0$ : nombre initial de noyaux radioactifs (à $t=0$).

### 2. Le temps de demi-vie ($t_{1/2}$)
> [!abstract] Définition
> Le temps de demi-vie $t_{1/2}$ est la durée nécessaire pour que la moitié des noyaux radioactifs initialement présents se soient désintégrés.
> $$N(t_{1/2}) = \frac{N_0}{2}$$

---

## IV - L'activité d'un échantillon

> [!info] Définition : Activité ($A$)
> L'activité d'un échantillon correspond au **nombre de désintégrations par seconde**.
> Elle s'exprime en **Becquerel (Bq)**. *1 Bq = 1 désintégration par seconde.*

L'activité est la dérivée (au signe près) du nombre de noyaux :
$$A(t) = -\frac{dN(t)}{dt}$$

En dérivant l'expression de $N(t) = N_0 \cdot e^{-\lambda t}$, on obtient :
$$A(t) = - (N_0 \cdot (-\lambda) \cdot e^{-\lambda t}) = \lambda \cdot N_0 \cdot e^{-\lambda t}$$

> [!formula] Évolution de l'activité
> En posant $A_0 = \lambda \cdot N_0$ (l'activité initiale), on s'aperçoit que l'activité suit exactement la même loi mathématique que la population de noyaux :
> $$A(t) = A_0 \cdot \exp(-\lambda \cdot t)$$

### Démonstration exigible : Lien entre $\lambda$ et $t_{1/2}$
On sait qu'à $t = t_{1/2}$, l'activité est divisée par 2 : $A(t_{1/2}) = \frac{A_0}{2}$.
En utilisant la loi de décroissance :
$$A_0 \cdot e^{-\lambda \cdot t_{1/2}} = \frac{A_0}{2}$$
$$e^{-\lambda \cdot t_{1/2}} = \frac{1}{2}$$
On applique le logarithme népérien ($\ln$) de chaque côté :
$$-\lambda \cdot t_{1/2} = \ln\left(\frac{1}{2}\right)$$
Comme $\ln(1/2) = -\ln(2)$ :
$$-\lambda \cdot t_{1/2} = -\ln(2)$$

> [!important] Relation fondamentale
> $$t_{1/2} = \frac{\ln(2)}{\lambda}$$