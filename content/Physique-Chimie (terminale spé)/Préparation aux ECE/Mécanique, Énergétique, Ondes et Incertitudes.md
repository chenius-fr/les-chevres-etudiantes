---
title: Mécanique, Énergétique, Ondes et Incertitudes
tags:
  - physique_chimie
  - terminale
  - ECE
  - TP
  - mécanique
  - ondes
  - incertitudes
---


---

## Mécanique et Pointage Vidéo

**Objectif :** Obtenir les équations horaires de la position, de la vitesse et de l'accélération d'un système en mouvement à partir d'une vidéo.

**Le protocole logiciel (LatisPro ou Atelier Scientifique) :**
1. **Étalonnage (Crucial) :** Indiquer au logiciel l'échelle réelle de la vidéo en sélectionnant un objet de longueur connue sur l'image (ex: une règle d'1 mètre) et en saisissant sa valeur.
2. **Origine et Axes :** Placer l'origine du repère (souvent au point de départ du mouvement) et orienter les axes (axe Y vers le haut en général).
3. **Pointage :** Cliquer précisément sur le centre de gravité du système image par image (le logiciel fait avancer la vidéo automatiquement).
4. **Traitement :** Utiliser le tableur/grapheur du logiciel pour créer les grandeurs dérivées :
   * Vitesse : $v_x = \frac{dx}{dt}$ et $v_y = \frac{dy}{dt}$.
   * Accélération : $a_x = \frac{dv_x}{dt}$ et $a_y = \frac{dv_y}{dt}$.

---

## Énergétique et Conservation

**Objectif :** Vérifier le principe de conservation de l'énergie mécanique.

> **Formules fondamentales**
> * **Énergie Cinétique :** $E_c = \frac{1}{2} m \cdot v^2$
> * **Énergie Potentielle de Pesanteur :** $E_{pp} = m \cdot g \cdot y$ *(si l'axe y est orienté vers le haut)*
> * **Énergie Mécanique :** $E_m = E_c + E_{pp}$

**Exploitation classique :**
* Si le système n'est soumis qu'à des forces conservatives (comme le poids) et qu'on néglige les frottements, l'énergie mécanique $E_m$ est **constante**. 
* Graphiquement, on observe une courbe de $E_c$ qui monte, une courbe de $E_{pp}$ qui descend (ou l'inverse), mais leur somme $E_m$ forme une ligne droite horizontale.

---

## Ondes (Diffraction et Interférences)

**Objectif :** Mesurer des dimensions microscopiques (comme l'épaisseur d'un cheveu) grâce aux ondes lumineuses.

### 1. Phénomène de Diffraction (Fente ou Fil simple)
Lorsqu'un laser de longueur d'onde $\lambda$ éclaire un obstacle de taille $a$ (fente ou fil), on observe une figure de diffraction sur un écran situé à une distance $D$.
> **Relation de la largeur de la tache centrale ($L$) :**
> À partir de l'écart angulaire $\theta = \frac{\lambda}{a}$ et de l'approximation des petits angles ($\tan \theta \approx \theta \approx \frac{L}{2D}$), on déduit :
> $$L = \frac{2 \lambda D}{a}$$
*(Astuce ECE : On trace souvent la courbe $L = f(\frac{1}{a})$ qui est une droite passant par l'origine, pour ensuite déterminer la taille d'un fil inconnu par lecture graphique).*

### 2. Phénomène d'Interférences (Fentes d'Young)
Lorsqu'un laser traverse deux fentes séparées par une distance $b$, on observe une alternance de franges brillantes et sombres.
> **Relation de l'interfrange ($i$) :**
> L'interfrange (distance entre deux milieux de franges brillantes consécutives) est :
> $$i = \frac{\lambda D}{b}$$
*(Logiciel ECE : On utilise souvent un logiciel de traitement d'image comme **Salsa J** pour mesurer la distance de plusieurs interfranges sur une photographie afin de réduire l'incertitude).*

---

## L'Effet Doppler

**Objectif :** Déterminer la vitesse d'une source sonore en mouvement.

* **Principe :** Le son perçu est plus aigu (fréquence plus élevée) quand la source s'approche, et plus grave (fréquence plus basse) quand elle s'éloigne.
* **Logiciel ECE (Audacity) :** On sélectionne une portion du signal sonore enregistré, puis on utilise l'outil d'analyse spectrale (ou on mesure une durée $\Delta t$ correspondant à $n$ motifs pour en déduire la période $T$ puis la fréquence $f = \frac{1}{T}$).
* **Calcul :** On utilise la formule du décalage Doppler ($\Delta f = f_{reçue} - f_{\text{émise}}$) combinée aux équations fournies dans le document ressource pour isoler la vitesse $v$.

---

## Calcul et Évaluation des Incertitudes

C'est l'étape de validation indispensable de tout TP.

### 1. Incertitude-type d'une mesure unique (Type B)
Lorsqu'on utilise un appareil de mesure, le constructeur ou la graduation induit une incertitude.
* **Appareil à graduation** (règle, éprouvette) : $u = \frac{\text{1 graduation}}{\sqrt{12}}$
* **Appareil avec tolérance constructeur** (fiole jaugée, pipette) : $u = \frac{\text{Tolérance}}{\sqrt{3}}$

### 2. Incertitude élargie et Présentation du résultat
Pour garantir le résultat avec un niveau de confiance (souvent 95%), on multiplie l'incertitude-type $u$ par un facteur d'élargissement $k$ (généralement $k=2$).
$$U(x) = k \times u(x)$$
> **Écriture finale exigée :**
> $$x = x_{\text{mesuré}} \pm U(x) \quad \text{avec son unité.}$$
*(Attention : $U(x)$ ne garde qu'**un seul chiffre significatif**, et la mesure $x$ s'arrondit à la même décimale).*

### 3. Écart relatif
Pour comparer une valeur expérimentale ($x_{exp}$) à une valeur théorique ($x_{th}$), on calcule l'écart relatif (en %) :
$$\text{Écart relatif} = \frac{|x_{exp} - x_{th}|}{x_{th}} \times 100$$
*(Si l'écart est inférieur à 5%, l'expérience est considérée comme très concluante).*

---

## La Démarche "Type ECE" face à un sujet vierge

Lorsque le sujet demande de proposer un protocole de A à Z :
1. **Identifier l'objectif :** Que cherche-t-on à mesurer ou à prouver ?
2. **Lister le matériel pertinent :** Choisir la verrerie la plus précise possible (verrerie jaugée préférée à la verrerie graduée).
3. **Rédiger par tirets :** Des phrases courtes avec des verbes d'action à l'infinitif.
4. **Schématiser :** Faire un schéma clair, grand et **légendé** du montage (ex: titrage ou circuit électrique).
5. **Justifier l'exploitation :** Expliquer brièvement comment les mesures permettront de répondre à la question (ex: "On tracera la courbe...", "À l'équivalence on appliquera la formule...").