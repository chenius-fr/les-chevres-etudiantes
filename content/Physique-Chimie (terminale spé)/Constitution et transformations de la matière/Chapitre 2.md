# Chapitre 2 : Équilibres Acide-Base
**Thème** : [[Constitution et transformations de la matière]]
**Tags** : #physique_chimie #terminale #cours #acide_base #pH

---

## I - Réactions Acide / Base

### 1. Définitions

> [!abstract] Définition : Acide selon Brønsted
> Un acide est une espèce chimique capable de **céder** au moins un proton $H^+$.
> *Exemples : acide citrique, vinaigre ($CH_3COOH$), acide chlorhydrique ($HCl$).*

> [!abstract] Définition : Base selon Brønsted
> Une base est une espèce chimique capable de **capter** au moins un proton $H^+$.
> *Exemples : ion éthanoate ($CH_3COO^-$), ion chlorure ($Cl^-$), ion hydroxyde ($HO^-$).*

**Couples Acide / Base :**
Un acide et une base sont dits conjugués lorsqu'ils sont liés par le transfert d'un ion $H^+$. On note le couple **Acide / Base**.
La demi-équation associée est :
$$AH \rightleftharpoons A^- + H^+$$

### 2. Espèces amphotères (ou ampholytes)

> [!info] Définition
> Une espèce chimique qui est l'acide d'un couple et la base d'un autre couple est dite **amphotère**.

* **L'eau ($H_2O$)** est l'ampholyte par excellence :
    * Base dans $H_3O^+ / H_2O$
    * Acide dans $H_2O / HO^-$

### 3. Réaction acide-base

> [!tldr] Propriété : Transfert de proton
> Une réaction acido-basique consiste en un transfert de proton(s) entre l'acide d'un couple 1 et la base d'un couple 2.
>
> $${A_1H}_{(aq)} + {A_2^-}_{(aq)} \rightleftharpoons {A_1^-}_{(aq)} + {A_2H}_{(aq)}$$

[Image de réaction acido-basique transfert de proton]

* **Réaction totale** : notée avec une flèche simple $\rightarrow$
* **Réaction équilibrée** : notée avec une double flèche $\rightleftharpoons$

### 4. Le pH

> [!formula] Définition : pH
> Le pH mesure l'acidité d'une solution aqueuse :
> $$pH = -\log([H_3O^+])$$
> *Inversement :* $[H_3O^+] = 10^{-pH}$

> [!tip] Point Math : Le Logarithme
> * $\log(10^a) = a$
> * $\log(a \times b) = \log(a) + \log(b)$
> * $\log\left(\frac{a}{b}\right) = \log(a) - \log(b)$

---

## II - Force des acides et des bases

### 1. Autoprotolyse de l'eau

> [!important] Produit ionique de l'eau $K_e$
> L'eau réagit sur elle-même selon l'équilibre : $2 H_2O_{(l)} \rightleftharpoons H_3O^+_{(aq)} + HO^-_{(aq)}$
>
> $$K_e = [H_3O^+] \cdot [HO^-] = 10^{-14} \quad (\text{à } 25^\circ\text{C})$$

### 2. Force d'un acide ou d'une base

* **Acide Fort** : Sa réaction avec l'eau est **totale** ($\tau = 1$).
* **Acide Faible** : Sa réaction avec l'eau est **limitée** ($\tau < 1$).

### 3. Constante d'acidité ($K_a$)

> [!formula] Constante d'acidité
> Pour un couple $AH/A^-$, la constante d'équilibre de la réaction avec l'eau est appelée constante d'acidité $K_a$ :
> $$K_a = \frac{[A^-]_{eq} \cdot [H_3O^+]_{eq}}{[AH]_{eq}}$$

On utilise souvent le **$pK_a$** pour comparer les forces :
$$pK_a = -\log(K_a) \quad \text{et} \quad K_a = 10^{-pKa}$$

---

## III - Prédominance

### 1. Relation fondamentale
D'après la définition du $K_a$, on peut établir la relation :
$$pH = pK_a + \log\left(\frac{[A^-]}{[AH]}\right)$$

### 2. Diagramme de prédominance

> [!check] Critères de prédominance
> * Si **$pH < pK_a$** : $[AH] > [A^-] \rightarrow$ **L'acide prédomine.**
> * Si **$pH > pK_a$** : $[A^-] > [AH] \rightarrow$ **La base prédomine.**
> * Si **$pH = pK_a$** : $[AH] = [A^-]$

[Image diagramme de prédominance acide base]

### 3. Indicateurs colorés
Un indicateur coloré possède une **zone de virage** située environ à $pH = pK_a \pm 1$. C'est l'endroit où sa couleur change car les concentrations de sa forme acide et basique deviennent comparables.

---

## IV - Cas particuliers : Solutions tampons

> [!info] Définition : Solution Tampon
> Une solution dont le pH varie très peu par ajout modéré d'acide, de base ou par dilution.
> *Exemple : Le sang humain (système tampon $CO_2,H_2O / HCO_3^-$).*

---
## 🧮 Outil Math : Second degré
Pour trouver l'avancement $x$ dans un équilibre complexe :
$$ax^2 + bx + c = 0 \implies \Delta = b^2 - 4ac$$
$$x = \frac{-b + \sqrt{\Delta}}{2a}$$