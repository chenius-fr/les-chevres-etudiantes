# Chapitre 8 : Cinétique Chimique
**Thème** : [[Constitution et transformations de la matière]]
**Tags** : #physique_chimie #terminale #cours #cinétique #vitesse #catalyse

---

## I - Les facteurs cinétiques

> [!abstract] Définitions
> * **Cinétique chimique** : C'est l'étude du déroulement temporel (la vitesse) des réactions chimiques et des facteurs qui la modifient.
> * **Facteurs cinétiques** : Paramètres physiques ou chimiques qui influencent la vitesse d'une réaction.

Les trois principaux facteurs cinétiques sont :
1. La température
2. La concentration des réactifs
3. Le catalyseur (ou la pression pour les gaz)

### 1. La température
> [!info] Propriété
> De manière générale, **plus la température augmente, plus la réaction est rapide**.
> * **Pour accélérer** : On utilise généralement un montage de **chauffage à reflux**.
> * **Pour stopper** : On réalise une **trempe** (refroidissement brutal, souvent avec un bain d'eau glacée). Cela permet de stopper la réaction à un instant précis pour faire une mesure (titrage).

### 2. La concentration des réactifs
> [!info] Propriété
> **Plus la concentration initiale des réactifs est élevée, plus la réaction est rapide.** Au cours d'une réaction classique, la vitesse diminue car les réactifs sont consommés.

> [!check] Bilan microscopique (Pourquoi ?)
> Pour que deux molécules réagissent, elles doivent s'entrechoquer.
> * L'augmentation de la **concentration** augmente la probabilité des chocs.
> * L'augmentation de la **température** augmente l'agitation thermique, et donc l'efficacité et l'énergie des chocs.

---

## II - La catalyse

> [!abstract] Définition : Catalyseur
> Un catalyseur est une espèce chimique qui **accélère une réaction** (en modifiant le mécanisme réactionnel), mais qui est **consommé puis régénéré**. Sa formule n'apparaît donc pas dans l'équation globale de la réaction.

Il existe 3 grands types de catalyse :
* **Catalyse homogène** : Le catalyseur est dans la *même phase* (même état physique) que les réactifs.
* **Catalyse hétérogène** : Le catalyseur n'est *pas dans la même phase* que les réactifs (ex: un métal solide dans un liquide).
* **Catalyse enzymatique** : Le catalyseur est une macromolécule biologique (une *enzyme*).

---

## III - Vitesses volumiques de réaction

### 1. Vitesse d'apparition et de disparition
Soit une réaction produisant un produit $P$ à partir d'un réactif $R$.

> [!formula] Vitesse volumique d'apparition d'un produit $P$
> La vitesse volumique d'apparition, notée $v_{app}(P)$, est la dérivée par rapport au temps de sa concentration :
> $$v_{app}(P) = \frac{d[P]}{dt}$$

> [!formula] Vitesse volumique de disparition d'un réactif $R$
> La vitesse volumique de disparition, notée $v_{disp}(R)$, est l'opposé de la dérivée par rapport au temps de sa concentration (pour obtenir une grandeur positive) :
> $$v_{disp}(R) = - \frac{d[R]}{dt}$$

### 2. Détermination graphique
> [!tip] Point Math : La dérivée
> Graphiquement, le nombre dérivé d'une fonction à un instant $t$ correspond au **coefficient directeur de la tangente** à la courbe à cet instant.

Pour calculer une vitesse à l'instant $t$ :
1. On trace la tangente à la courbe à l'abscisse $t$.
2. On choisit deux points $A(x_A, y_A)$ et $B(x_B, y_B)$ sur cette tangente (les plus éloignés possibles pour plus de précision).
3. On calcule le coefficient directeur : $a = \frac{\Delta y}{\Delta x} = \frac{y_B - y_A}{x_B - x_A}$

---

## IV - Temps de demi-réaction et Loi d'ordre 1

### 1. Le temps de demi-réaction ($t_{1/2}$)
> [!abstract] Définition
> Le temps de demi-réaction, noté $t_{1/2}$, est la durée nécessaire pour que l'avancement $x$ atteigne la moitié de son avancement final $x_f$ :
> $$x(t_{1/2}) = \frac{x_f}{2}$$
> *(Si la réaction est totale et qu'il n'y a qu'un réactif $A$, c'est le temps au bout duquel la concentration de $A$ a été divisée par 2 : $[A](t_{1/2}) = \frac{[A]_0}{2}$).*

### 2. Réaction d'ordre 1
> [!info] Définition
> Une réaction est dite d'ordre 1 par rapport à un réactif $A$ (si $B$ est en large excès) lorsque sa vitesse volumique de disparition est **proportionnelle** à sa concentration.

> [!formula] Équation différentielle d'ordre 1
> $$v_{disp}(A) = k \cdot [A]$$
> Ce qui se traduit mathématiquement par l'équation différentielle :
> $$- \frac{d[A]}{dt} = k \cdot [A] \iff \frac{d[A]}{dt} + k \cdot [A] = 0$$
> *avec $k$ : constante de vitesse (en $\text{s}^{-1}$ ou $\text{min}^{-1}$).*

La solution de cette équation différentielle est une fonction exponentielle décroissante :
$$[A]_t = [A]_0 \cdot \exp(-k \cdot t)$$

### 3. Point Méthode : Comment prouver qu'une réaction est d'ordre 1 ?
Pour démontrer qu'une réaction est d'ordre 1, on peut utiliser l'une des 3 méthodes suivantes :
* **Méthode 1 (Graphique $t_{1/2}$)** : Montrer graphiquement que le temps de demi-réaction $t_{1/2}$ est **indépendant** de la concentration initiale $[A]_0$ (si on divise plusieurs fois la concentration par 2, l'intervalle de temps est toujours le même).
* **Méthode 2 (Vitesses)** : Vérifier que $v_{disp}$ (ou $v_{app}$) est **proportionnelle** à $[A]$ (en traçant $v = f([A])$, on doit obtenir une droite passant par l'origine).
* **Méthode 3 (Modélisation numérique)** : Montrer que la courbe d'évolution de la concentration est modélisable par la fonction mathématique $[A]_t = [A]_0 \cdot \exp(-k \cdot t)$.