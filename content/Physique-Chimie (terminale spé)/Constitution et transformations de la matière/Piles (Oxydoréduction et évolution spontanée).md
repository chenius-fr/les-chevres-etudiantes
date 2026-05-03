---
title: Piles (Oxydoréduction et évolution spontanée)
tags:
  - physique_chimie
  - terminale
  - cours
  - rédox
  - pile
---

**Thème** : [[Constitution et transformations de la matière]]

---

## I - Rappels d'Oxydo-réduction

### 1. Le couple Rédox

> [!abstract] Définitions
> * **Oxydant** : C'est une espèce chimique capable de **capter** un (ou plusieurs) électron(s) $e^-$.
> * **Réducteur** : C'est une espèce chimique capable de **céder** un (ou plusieurs) électron(s) $e^-$.
> * **Couple Oxydant/Réducteur (Rédox)** : C'est un ensemble formé par un oxydant et un réducteur qui appartiennent au même élément chimique, noté conventionnellement **Ox/Réd**.

*Exemples classiques :*
* $Fe^{3+} / Fe^{2+}$
* $I_2 / I^-$
* $MnO_4^- / Mn^{2+}$
* $Cu^{2+} / Cu$

On associe à chaque couple une demi-équation indiquant les électrons transférés :
$$Ox + n \cdot e^- \rightleftharpoons Réd$$
*Exemples :* $Cu^{2+}_{(aq)} + 2e^- \rightleftharpoons Cu_{(s)}$ et $2H^+_{(aq)} + 2e^- \rightleftharpoons H_{2(g)}$.

### 2. Méthode pour équilibrer une demi-équation
Pour écrire correctement la demi-équation de l'oxydant vers le réducteur (en milieu acide) :
1. Écrire l'égalité : $\text{Oxydant} = \text{Réducteur}$.
2. Équilibrer tous les atomes **autres** que l'oxygène ($O$) et l'hydrogène ($H$).
3. Équilibrer les atomes d'oxygène ($O$) en ajoutant des molécules d'eau **$H_2O$**.
4. Équilibrer les atomes d'hydrogène ($H$) en ajoutant des protons **$H^+$**.
5. Équilibrer enfin les charges électriques en ajoutant des électrons **$e^-$** du côté de l'oxydant.

### 3. L'équation de réaction globale
> [!tip] Méthode
> 1. Écrire les 2 demi-équations des deux couples impliqués.
> 2. Repérer les **réactifs** (ceux présents initialement) et les placer à gauche.
> 3. Vérifier le nombre d'électrons échangés. Si nécessaire, multiplier les demi-équations par des coefficients croisés pour que le nombre d'électrons cédés soit égal au nombre d'électrons captés.
> 4. Additionner les deux équations (les électrons doivent s'annuler et disparaître du bilan final).
> 5. Simplifier les espèces présentes des deux côtés (comme l'eau ou les $H^+$).

---

## II - L'évolution spontanée d'un système

### 1. Le quotient de réaction ($Q_r$)
Considérons l'équation de réaction en solution aqueuse suivante :
$$aA_{(aq)} + bB_{(aq)} \rightleftharpoons cC_{(aq)} + dD_{(aq)}$$

> [!formula] Le quotient de réaction
> Le quotient de réaction $Q_r$ (sans unité) d'un système à un instant $t$ est défini par :
> $$Q_r = \frac{\left(\frac{[C]}{C^\circ}\right)^c \times \left(\frac{[D]}{C^\circ}\right)^d}{\left(\frac{[A]}{C^\circ}\right)^a \times \left(\frac{[B]}{C^\circ}\right)^b}$$
> *Avec $C^\circ = 1 \text{ mol}\cdot\text{L}^{-1}$ (concentration standard, indispensable pour que $Q_r$ n'ait pas de dimension).*

> [!warning] Règle fondamentale pour $Q_r$
> Le **solvant** (généralement l'eau liquide $H_2O_{(l)}$) et les **solides** ($S_{(s)}$) n'interviennent pas dans l'expression de $Q_r$ (on les remplace par le chiffre $1$).

### 2. Le sens d'évolution

> [!important] La constante d'équilibre ($K$)
> À l'état d'équilibre, le quotient de réaction $Q_r$ ne varie plus et atteint une valeur fixe appelée **constante d'équilibre $K$**.
> $$K = Q_{r, eq}$$
> *La valeur de $K$ ne dépend que de la température.*

Pour prévoir le sens d'évolution spontanée d'un système, on compare le $Q_r$ initial avec la constante $K$ :
* Si **$Q_r < K$** : Le système évolue dans le **sens direct** ($\rightarrow$). Les réactifs se consomment pour former des produits.
* Si **$Q_r > K$** : Le système évolue dans le **sens indirect** ($\leftarrow$). Les produits réagissent pour reformer les réactifs.
* Si **$Q_r = K$** : Le système est à l'**équilibre** (plus d'évolution macroscopique).
---

## III - Constitution et fonctionnement d'une Pile

### 1. Principe d'une pile
> [!abstract] Définition
> * **Demi-pile** : Association des deux espèces d'un couple rédox (ex: une plaque de métal plongeant dans une solution de ses propres ions).
> * **Pile** : Dispositif constitué de deux demi-piles reliées entre elles. Elle permet de convertir de l'énergie chimique en énergie électrique grâce à un **transfert spontané et indirect** d'électrons.

**Vocabulaire des électrodes (Moyen mnémotechnique) :**
* **Anode** = **O**xydation *(les deux mots commencent par une voyelle)*.
* **Cathode** = **R**éduction *(les deux mots commencent par une consonne)*.

*Sur le schéma d'une pile (ex: Pile Daniell) :*
* Les électrons $e^-$ circulent dans les fils métalliques de l'anode ($\Theta$) vers la cathode ($\oplus$).
* Le courant électrique $I$ circule conventionnellement dans le sens inverse des électrons : de la cathode ($\oplus$) vers l'anode ($\Theta$).

### 2. Le Pont Salin
> [!info] Rôle du pont salin
> Le pont salin (ou jonction électrolytique) relie les deux demi-piles et possède deux fonctions indispensables :
> 1. **Fermer le circuit électrique** pour permettre le passage du courant.
> 2. **Assurer l'électroneutralité** des solutions (les ions positifs cationiques migrent vers la cathode, et les ions négatifs anioniques migrent vers l'anode pour compenser la création/consommation d'ions lors de la réaction).

### 3. Capacité électrique d'une pile ($Q_{max}$)
La pile s'arrête de débiter du courant (elle est "usée") lorsque le système atteint l'équilibre chimique ($Q_r = K$) ou, plus couramment, lorsque le **réactif limitant** est totalement consommé.

> [!formula] Capacité maximale ($Q_{max}$)
> C'est la charge électrique maximale (quantité totale d'électricité) que la pile peut débiter :
> $$Q_{max} = n(e^-)_{max} \times N_A \times e$$
> 
> * $Q_{max}$ en Coulombs ($\text{C}$) ou en Ampère-heure ($\text{A}\cdot\text{h}$)
> * $n(e^-)_{max}$ : quantité de matière maximale d'électrons échangés (en $\text{mol}$), déterminée grâce au tableau d'avancement et au réactif limitant.
> * $N_A$ : Constante d'Avogadro ($\simeq 6,02 \times 10^{23} \text{ mol}^{-1}$)
> * $e$ : Charge élémentaire ($\simeq 1,6 \times 10^{-19} \text{ C}$)
> 
> *Remarque* : Le produit $N_A \times e$ est appelé Constante de Faraday ($F \simeq 96500 \text{ C}\cdot\text{mol}^{-1}$). On peut donc écrire : $Q_{max} = n(e^-)_{max} \times F$.