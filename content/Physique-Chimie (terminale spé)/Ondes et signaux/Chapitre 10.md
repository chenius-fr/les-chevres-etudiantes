# Chapitre 10 : Propagation des ondes
**Thème** : [[Ondes et signaux]]
**Tags** : #physique_chimie #terminale #cours #ondes #doppler #diffraction #interférences

---

## I - Généralités sur les ondes

> [!abstract] Définition : Onde
> Une onde est la propagation d'une perturbation, **avec déplacement d'énergie mais sans déplacement de matière**.

Il existe 2 grandes catégories d'ondes :
1. **Les ondes mécaniques** : Elles ont besoin d'un milieu matériel pour se propager (ex: le son, les vagues, les ondes sismiques).
2. **Les ondes électromagnétiques (OEM)** : Elles se propagent dans le vide mais aussi dans les milieux matériels (ex: la lumière).

> [!tip] Les spectres à connaître
> * **Spectre sonore** : Infrasons ($< 20 \text{ Hz}$) | **Son audible** | Ultrasons ($> 20 \text{ kHz}$)
> * **Spectre OEM** : Ondes radio | Micro-ondes | IR | **Lumière visible** | UV | Rayons X | Rayons $\gamma$

> [!formula] Le retard ($\tau$)
> Si une perturbation passe par un point $M_1$ à l'instant $t_1$, puis par un point $M_2$ à l'instant $t_2$, le retard $\tau$ est le temps mis par l'onde pour parcourir la distance $M_1M_2$.
> La vitesse de propagation (ou célérité) $v$ de l'onde est :
> $$v = \frac{M_1M_2}{\tau}$$

---

## II - Ondes Progressives Périodiques Sinusoïdales (OPPS)

Une OPPS possède une **double périodicité** :
* **Périodicité temporelle ($T$)** : La période $T$ (en secondes) est la durée nécessaire pour qu'un point de l'espace repasse par la même position et dans le même sens.
* **Périodicité spatiale ($\lambda$)** : La longueur d'onde $\lambda$ (en mètres) est la plus petite distance séparant deux points vibrant en phase. C'est aussi la distance parcourue par l'onde durant une période $T$.

> [!formula] Relation fondamentale
> La vitesse de propagation fait le lien entre les deux périodicités :
> $$v = \frac{\lambda}{T} = \lambda \cdot f$$
> *avec $f$ la fréquence de l'onde en Hertz (Hz), sachant que $f = \frac{1}{T}$.*

---

## III - Le domaine de l'acoustique (Ondes sonores)

### 1. Intensité et Niveau d'intensité sonore

> [!info] Intensité sonore ($I$)
> L'intensité sonore, notée $I$, s'exprime en $\text{W}\cdot\text{m}^{-2}$. Elle correspond à la puissance $P$ de l'onde répartie sur une surface $S$.
> $$I = \frac{P}{S}$$
> *L'intensité d'audibilité minimale est $I_0 = 10^{-12} \text{ W}\cdot\text{m}^{-2}$.*

L'amplitude des sons est très grande (de $10^{-12}$ à plus de $1$), on utilise donc une échelle logarithmique pour se rapprocher de la perception de l'oreille humaine : le niveau d'intensité sonore.

> [!formula] Niveau d'intensité sonore ($L$)
> Le niveau d'intensité sonore, noté $L$, s'exprime en décibels (dB).
> $$L = 10 \cdot \log\left(\frac{I}{I_0}\right)$$
> *Inversement :* $I = I_0 \cdot 10^{\frac{L}{10}}$

> [!warning] Attention : Règle d'additivité
> L'intensité sonore $I$ est liée à l'énergie, elle est **additive** ($I_{totale} = I_1 + I_2$).
> Le niveau sonore $L$ **n'est pas une grandeur additive** ! ($L_{totale} \neq L_1 + L_2$).
> *Exemple : Si $L_1 = 70\text{ dB}$ et $L_2 = 70\text{ dB}$, le son perçu sera de $73\text{ dB}$ (car l'intensité est multipliée par 2, ce qui ajoute $\log(2) \times 10 \approx +3\text{ dB}$).*

### 2. Atténuation
* **Atténuation géométrique** : L'intensité diminue car l'énergie se répartit sur une surface de plus en plus grande à mesure qu'on s'éloigne de la source. ($A = L_{proche} - L_{\text{éloigné}}$).
* **Atténuation par absorption** : L'onde est absorbée en traversant un milieu ou une paroi. ($A = L_{incident} - L_{transmis}$).

---

## IV - L'Effet Doppler

> [!abstract] Définition
> L'effet Doppler est la modification de la fréquence perçue d'une onde (mécanique ou électromagnétique) liée au mouvement relatif de la source et du récepteur. 

> [!check] Règle générale
> Soit $\Delta f = f_{per\text{ç}ue} - f_{\text{émise}}$.
> * **Rapprochement** : La fréquence perçue est plus élevée (le son est plus aigu). Donc $\Delta f > 0$.
> * **Éloignement** : La fréquence perçue est plus faible (le son est plus grave). Donc $\Delta f < 0$.
> 
> *Plus la vitesse relative est grande, plus le décalage $|\Delta f|$ est grand. Cela sert notamment pour les radars routiers ou l'astrophysique (décalage vers le rouge des galaxies, dit "Redshift").*

---

## V - Optique ondulatoire : Diffraction et Interférences

Ces deux phénomènes sont la preuve irréfutable du caractère ondulatoire de la lumière.

### 1. La Diffraction
> [!info] Définition
> La diffraction est la modification de la direction de propagation d'une onde lorsqu'elle rencontre un obstacle ou une fente.
> **Condition** : Le phénomène est marqué si la taille de l'obstacle ($a$) est du même ordre de grandeur ou inférieure à la longueur d'onde ($\lambda$).

> [!formula] Écart angulaire ($\theta$)
> Pour une fente rectangulaire de largeur $a$ :
> $$\theta = \frac{\lambda}{a}$$
> *(Pour une ouverture circulaire de diamètre $d$, la formule est $\theta = 1,22 \frac{\lambda}{d}$)*

**Démonstration de la largeur de la tache centrale ($L$) :**
D'après un schéma géométrique, avec un écran placé à une distance $D$, on a : $\tan(\theta) = \frac{L/2}{D}$.
Pour de petits angles (en radians), $\tan(\theta) \approx \theta$.
Donc $\theta = \frac{L}{2D}$. En égalisant avec la formule de l'écart angulaire : $\frac{L}{2D} = \frac{\lambda}{a}$

> $$L = \frac{2 \cdot \lambda \cdot D}{a}$$
> *La largeur de la tache centrale est proportionnelle à $\lambda$ et $D$, et inversement proportionnelle à la largeur de la fente $a$.*

### 2. Les Interférences
> [!abstract] Définition et Conditions
> Les interférences se produisent lorsque deux ondes se superposent (leurs amplitudes s'additionnent).
> **Condition** : Les ondes doivent être **cohérentes** (même nature, même fréquence, et présenter un déphasage constant, ce qui est généralement obtenu en divisant une source unique comme dans l'expérience des fentes d'Young).

On définit la différence de marche (ou différence de chemin optique) $\delta = S_2M - S_1M$.
* **Interférences constructives** : Les ondes arrivent en phase (les amplitudes s'ajoutent pour donner une frange brillante).
  > $$\delta = k \cdot \lambda \quad (\text{avec } k \in \mathbb{Z})$$
* **Interférences destructives** : Les ondes arrivent en opposition de phase (les amplitudes s'annulent pour donner une frange sombre).
  > $$\delta = \left(k + \frac{1}{2}\right) \cdot \lambda \quad (\text{avec } k \in \mathbb{Z})$$

> [!formula] L'interfrange ($i$)
> L'interfrange est la distance séparant deux franges brillantes (ou deux franges sombres) consécutives.
> $$i = \frac{\lambda \cdot D}{b}$$
> *avec $b$ (ou $e$, selon les notations) la distance séparant les deux sources secondaires (les deux fentes).*