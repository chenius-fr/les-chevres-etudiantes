# Chapitre 14 : Circuit RC
**Thème** : [[Ondes et signaux]] 
**Tags** : #physique_chimie #terminale #cours #électricité #circuit_RC #équa_diff

---

## I - Rappels et lois en électricité

### 1. Notations et grandeurs
> [!abstract] Définitions
> * **Dipôle** : Un composant électrique possédant deux pôles. Il en existe de très nombreux aux propriétés différentes (lampe, pile/générateur, résistance, LED, diode, condensateur).
> * Aux bornes d'un dipôle, on mesure une **tension $U_{AB}$** (en Volts, V).
> * Un dipôle est traversé par un **courant $I$** ou $i(t)$ (en Ampères, A).

**Conventions d'orientation :**
* **Convention récepteur** : La flèche de la tension $U$ et la flèche du courant $I$ sont de **sens inverses**.
* **Convention générateur** : La flèche de la tension $U$ et la flèche du courant $I$ sont dans le **même sens**.

### 2. Principales lois de l'électricité
> [!formula] La loi d'Ohm
> Dans un dipôle ohmique de résistance $R$ traversé par un courant $i$ en convention récepteur :
> $$u_R = R \cdot i$$
> * $R$ s'exprime en Ohms ($\Omega$).

> [!important] Loi des nœuds et Loi des mailles
> * **Loi des nœuds** : Pour un nœud du circuit, la somme des courants entrants est égale à la somme des courants sortants.
> * **Loi des mailles** : Pour une maille du circuit (une boucle fermée), la somme algébrique des tensions est nulle en faisant le tour dans le même sens. 
> *Exemple : $E - u_R - u_c = 0$*

---

## II - Le Condensateur

### 1. Propriétés
> [!info] Définition
> Un condensateur est un dipôle constitué de 2 plaques métalliques (appelées **armatures**) séparées par un isolant (appelé **diélectrique**). 
> Lorsqu'il est alimenté, le condensateur se charge : des charges électriques s'accumulent sur ses armatures.

### 2. Relations fondamentales
> [!formula] Charge et Tension
> La charge électrique $q_A$ (en Coulombs, C) portée par l'armature A est proportionnelle à la tension $u_c$ à ses bornes :
> $$q_A = C \cdot u_c$$
> * $C$ : **Capacité** du condensateur en Farads (F).

> [!formula] Intensité et Charge
> L'intensité du courant $i$ correspond au débit de charges électriques :
> $$i = \frac{dq_A}{dt}$$

En combinant ces deux relations (sachant que $C$ est une constante), on obtient la relation fondamentale du condensateur en convention récepteur :
$$i = \frac{d(C \cdot u_c)}{dt} \implies i = C \cdot \frac{du_c}{dt}$$

---

## III - Étude du Circuit RC

Un circuit RC est l'association en série d'un générateur idéal de tension $E$, d'une résistance $R$ et d'un condensateur de capacité $C$.

### 1. La charge du condensateur
Le condensateur est initialement déchargé ($u_c(0) = 0$). À $t=0$, on ferme l'interrupteur.

**Établissement de l'équation différentielle :**
1. D'après la loi des mailles : $E - u_R - u_c = 0$
2. D'après la loi d'Ohm : $u_R = R \cdot i \implies E - R \cdot i - u_c = 0$
3. D'après les propriétés du condensateur : $i = C \frac{du_c}{dt}$
4. On remplace : $E - R \cdot C \frac{du_c}{dt} - u_c = 0$

En réorganisant pour isoler la dérivée, on obtient l'équation différentielle vérifiée par $u_c$ :
> [!important] Équation différentielle (Charge)
> $$\frac{du_c}{dt} + \frac{1}{R \cdot C} u_c = \frac{E}{R \cdot C}$$

La solution de cette équation différentielle est de la forme :
$$u_c(t) = E \cdot (1 - e^{-\frac{t}{R \cdot C}})$$

### 2. La décharge du condensateur
Une fois chargé ($u_c(0) = E$), on bascule l'interrupteur pour exclure le générateur. Le condensateur se décharge dans la résistance.

**Établissement de l'équation différentielle :**
1. Loi des mailles (sans générateur) : $u_R + u_c = 0$
2. On applique la même méthode ($u_R = R \cdot i$ et $i = C \frac{du_c}{dt}$) :
   $$R \cdot C \frac{du_c}{dt} + u_c = 0$$

> [!important] Équation différentielle (Décharge)
> $$\frac{du_c}{dt} + \frac{1}{R \cdot C} u_c = 0$$

La solution de cette équation différentielle est de la forme :
$$u_c(t) = E \cdot e^{-\frac{t}{R \cdot C}}$$

---

## IV - La Constante de Temps ($\tau$)

### 1. Définition
> [!abstract] La constante de temps
> On remarque que le terme $R \cdot C$ est homogène à un temps (il s'exprime en secondes). On pose la constante de temps du circuit RC :
> $$\tau = R \cdot C$$
> Elle permet d'évaluer la rapidité de la charge ou de la décharge. Le régime permanent (fin de la charge/décharge) est atteint au bout d'environ $5\tau$.

### 2. Détermination graphique de $\tau$
Il existe deux méthodes pour déterminer $\tau$ à partir du graphique $u_c = f(t)$ :

> [!tip] Méthode 1 : Les 63% / 37%
> * **Lors de la charge** : $\tau$ est l'abscisse du point de la courbe d'ordonnée $u_c = 0,63 \times E$ (le condensateur est chargé à 63%).
> * **Lors de la décharge** : $\tau$ est l'abscisse du point de la courbe d'ordonnée $u_c = 0,37 \times E$ (il ne reste que 37% de la charge initiale).

> [!tip] Méthode 2 : La tangente à l'origine
> * On trace la tangente à la courbe à l'instant $t=0$. 
> * **Lors de la charge** : L'intersection de cette tangente avec l'asymptote horizontale $u_c = E$ donne pour abscisse $t = \tau$.
> * **Lors de la décharge** : L'intersection de cette tangente avec l'axe des abscisses ($u_c = 0$) donne $t = \tau$.