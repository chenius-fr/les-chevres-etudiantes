# Chapitre 15 : Mécanique des fluides
**Thème** : [[Mouvement et interactions]]
**Tags** : #physique_chimie #terminale #cours #mécanique #fluides #bernoulli #archimède

---

## Introduction : Rappel de Statique des fluides

> [!formula] Loi fondamentale de la statique des fluides
> Pour un fluide immobile et incompressible de masse volumique $\rho$, la différence de pression entre deux points A et B dépend uniquement de leur différence de hauteur $h$ :
> $$P_B = P_A + \rho \cdot g \cdot h$$
> * $P$ : Pression en Pascals (Pa)
> * $\rho$ : Masse volumique du fluide en $\text{kg}\cdot\text{m}^{-3}$ (Pour l'eau : $\rho \simeq 1000 \text{ kg}\cdot\text{m}^{-3}$)
> * $g$ : Intensité de la pesanteur ($\simeq 9,81 \text{ m}\cdot\text{s}^{-2}$)
> * $h$ : Différence d'altitude (profondeur) en mètres (m)

---

## I - La Poussée d'Archimède

Considérons un objet de volume $V$ et de masse $m$ plongé dans un fluide de masse volumique $\rho_{fluide}$.

> [!abstract] Définition : Poussée d'Archimède ($\vec{\Pi}_A$)
> Tout corps plongé dans un fluide au repos subit une force verticale, dirigée de bas en haut, opposée au **poids du volume de fluide déplacé**.

**Démonstration par l'équilibre :**
1. On imagine une portion de fluide (de même forme que l'objet) en équilibre au sein du fluide.
2. D'après la 2ème loi de Newton : $\sum \vec{F}_{ext} = \vec{0} \implies \vec{P}_{fluide} + \vec{\Pi}_A = \vec{0}$
3. Donc $\vec{\Pi}_A = - \vec{P}_{fluide} = - m_{fluide} \cdot \vec{g}$

> [!formula] Expression de la Poussée d'Archimède
> $$\vec{\Pi}_A = - \rho_{fluide} \cdot V_{immerg\acute{e}} \cdot \vec{g}$$
> 
> En valeur (norme) :
> $$\Pi_A = \rho_{fluide} \cdot V_{immerg\acute{e}} \cdot g$$

> [!tip] Cas de l'iceberg (Flottaison)
> Si un objet flotte, il est à l'équilibre. Son poids $\vec{P}$ est exactement compensé par la poussée d'Archimède $\vec{\Pi}_A$. 
> $$P = \Pi_A \iff \rho_{objet} \cdot V_{total} \cdot g = \rho_{fluide} \cdot V_{immerg\acute{e}} \cdot g$$
> On en déduit le pourcentage immergé : $\frac{V_{immerg\acute{e}}}{V_{total}} = \frac{\rho_{objet}}{\rho_{fluide}}$.

---

## II - Écoulement d'un fluide en régime permanent

Dans cette partie, on étudie un fluide en mouvement (régime permanent : la vitesse en un point donné de l'espace ne dépend pas du temps).

### 1. Le débit volumique ($D_v$)
> [!info] Définition
> Le débit volumique correspond au volume de fluide qui traverse une section $S$ d'une conduite par unité de temps.

> [!formula] Formules du débit volumique
> $$D_v = \frac{V}{\Delta t}$$
> $$D_v = S \cdot v$$
> * $D_v$ en $\text{m}^3\cdot\text{s}^{-1}$
> * $V$ : volume en $\text{m}^3$
> * $S$ : section (aire) de la conduite en $\text{m}^2$
> * $v$ : vitesse d'écoulement du fluide en $\text{m}\cdot\text{s}^{-1}$

### 2. Écoulement incompressible (Conservation du débit)
> [!important] Propriété
> Pour un fluide **incompressible** (comme les liquides), le débit volumique se conserve tout au long de la conduite.
> $$D_{v1} = D_{v2} \implies S_1 \cdot v_1 = S_2 \cdot v_2 = \text{constante}$$

*Conséquence directe* : Si une canalisation se resserre ($S_2 < S_1$), la vitesse du fluide augmente ($v_2 > v_1$). Le fluide accélère dans les rétrécissements.

---

## III - Relation de Bernoulli et Effet Venturi

La relation de Bernoulli traduit la **conservation de l'énergie mécanique** pour une particule de fluide incompressible en écoulement, en l'absence de frottements (fluide parfait).

### 1. La relation de Bernoulli

> [!formula] Équation de Bernoulli
> Le long d'une ligne de courant, entre un point A et un point B, on a :
> $$\frac{1}{2}\rho \cdot v_A^2 + \rho \cdot g \cdot z_A + P_A = \frac{1}{2}\rho \cdot v_B^2 + \rho \cdot g \cdot z_B + P_B = \text{constante}$$
> 
> L'équation est composée de trois termes (tous homogènes à une pression, en Pascals) :
> * $\frac{1}{2}\rho \cdot v^2$ : Pression dynamique (liée à l'énergie cinétique)
> * $\rho \cdot g \cdot z$ : Pression de pesanteur (liée à l'énergie potentielle)
> * $P$ : Pression statique

### 2. Application : L'effet Venturi
Considérons une conduite **horizontale** ($z_A = z_B$) qui présente un rétrécissement. 
L'équation de Bernoulli se simplifie :
$$\frac{1}{2}\rho \cdot v_A^2 + P_A = \frac{1}{2}\rho \cdot v_B^2 + P_B$$

D'après la conservation du débit, dans le rétrécissement (point B), la vitesse augmente ($v_B > v_A$).
Pour que l'égalité de Bernoulli reste vraie, il faut obligatoirement que la pression statique diminue ($P_B < P_A$).

> [!important] Conclusion : L'effet Venturi
> L'accélération d'un fluide entraîne inévitablement une **diminution de sa pression**.
> 
> *Exemple d'application (Trompe à eau / Fiole à vide)* : En faisant couler de l'eau très vite dans un tube rétréci, on crée une forte dépression. Si on connecte un tuyau à cet endroit, l'air est aspiré (principe utilisé pour la filtration sous vide avec un filtre Büchner).

