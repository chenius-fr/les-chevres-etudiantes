---
title: Titrages, Cinétique et Synthèse Organique
tags:
  - physique_chimie
  - terminale
  - ECE
  - TP
  - chimie
  - titrage
  - cinétique
  - synthèse
---


---

## Les Titrages (pH, Conductimétrie, Colorimétrie)

**Objectif :** Déterminer la concentration inconnue d'une solution (titrée) en la faisant réagir avec une solution de concentration connue (titrante).

### 1. Le Montage (À connaître par cœur)
* **En haut :** Potence, noix de serrage, et **burette graduée** contenant la solution **titrante** (concentration connue). *Attention : toujours faire le "zéro" en bas du ménisque.*
* **En bas :** Bécher ou erlenmeyer contenant un volume précis $V$ de la solution **titrée** (prélevé à la pipette jaugée), posé sur un **agitateur magnétique** avec un barreau aimanté à l'intérieur.
* **Capteurs :** Sonde pH-métrique ou conductimétrique plongeant dans le bécher (attention à ce que le barreau aimanté ne heurte pas la sonde !).

### 2. Le repérage de l'équivalence
L'équivalence est le moment où les réactifs ont été introduits dans les proportions stœchiométriques (ils sont tous les deux limitants).

* **Titrage Colorimétrique :** Repéré par un changement de couleur persistant à la goutte près (souvent grâce à un indicateur coloré dont la zone de virage encadre le pH à l'équivalence).
* **Titrage pH-métrique :** Repéré par un saut de pH.
  * *Méthode des tangentes :* Tracer deux tangentes parallèles de part et d'autre du saut, puis une troisième droite équidistante. Son intersection avec la courbe donne le point d'équivalence $E(V_{E} ; pH_{E})$.
  * *Courbe dérivée :* Tracer $\frac{dpH}{dV}$. L'équivalence correspond au pic (extremum) de la courbe.
* **Titrage Conductimétrique :** Repéré par une rupture de pente. On trace deux droites modélisant les deux parties de la courbe. Leur intersection donne le volume équivalent $V_{E}$.

> **Le calcul final (Relation à l'équivalence)**
> Pour une équation de la forme : $aA + bB \to Produits$
> À l'équivalence, on a :
> $$\frac{n_A}{a} = \frac{n_B}{b} \iff \frac{C_A \times V_A}{a} = \frac{C_B \times V_{E}}{b}$$

---

## Suivi Cinétique et $t_{1/2}$

**Objectif :** Étudier la vitesse d'une réaction chimique au cours du temps.

### 1. Les Facteurs Cinétiques
Un facteur cinétique est un paramètre qui modifie la vitesse d'une réaction :
* **La Température :** Plus elle est élevée, plus la réaction est rapide (agitation thermique). *Application ECE : bain-marie pour accélérer, bain d'eau glacée pour faire une "trempe" (stopper la réaction).*
* **La Concentration des réactifs :** Plus elle est élevée, plus la probabilité de chocs efficaces est grande.
* **Le Catalyseur :** Espèce chimique qui accélère la réaction sans être consommée au bilan final.

### 2. Le temps de demi-réaction ($t_{1/2}$)
> **Définition stricte**
> Le temps de demi-réaction $t_{1/2}$ est la durée nécessaire pour que l'avancement de la réaction atteigne **la moitié de sa valeur finale**.
> $$x(t_{1/2}) = \frac{x_f}{2}$$

**Méthode de lecture graphique :**
1. Repérer l'asymptote horizontale de la courbe (valeur finale $x_f$ ou concentration finale).
2. Diviser cette valeur par 2 sur l'axe des ordonnées.
3. Tracer une droite horizontale jusqu'à couper la courbe.
4. Lire l'abscisse correspondante : c'est $t_{1/2}$.

---

## Synthèse Organique

**Objectif :** Fabriquer une nouvelle molécule organique (comme la dibenzalacétone, le paracétamol, etc.).

### 1. Le Chauffage à Reflux
* **But :** Accélérer la réaction en chauffant (facteur cinétique), **sans perte de matière** (les vapeurs sont refroidies et retombent dans le ballon).
* **Montage :** Chauffe-ballon sur un support élévateur (pour la sécurité, pouvoir le baisser vite), ballon contenant le mélange et des grains de pierre ponce (pour réguler l'ébullition), surmonté d'un **réfrigérant à eau**.
* *Règle d'or :* L'eau froide entre toujours par le **bas** du réfrigérant et ressort par le **haut**.

### 2. L'isolement : Filtration sous vide (Büchner)
* **But :** Séparer très rapidement un produit solide du solvant liquide.
* **Matériel :** Fiole à vide reliée à une trompe à eau (qui crée l'aspiration), surmontée d'un entonnoir Büchner muni d'un papier filtre.
* **Étape clé :** On rince toujours le solide avec un solvant **froid** pour éliminer les impuretés sans redissoudre le produit de synthèse.

### 3. Le Rendement ($\eta$)
> **Formule du rendement**
> C'est le rapport entre la quantité réellement obtenue à la fin du TP et la quantité théorique maximale qu'on aurait pu obtenir si la réaction était totale (nécessite de trouver le réactif limitant avec un tableau d'avancement).
> $$\eta = \frac{n_{exp}}{n_{max}} = \frac{m_{exp}}{m_{max}}$$
> *(Le résultat est toujours compris entre 0 et 1, soit entre 0% et 100%).*