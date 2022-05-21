<!--
2022-04-12.22:53:58, Création :
    ~/prj/20210206.taxonomie-analyse-complexe/README.md
-->


# Taxonomie d’analyse complexe

- [Introduction](#introduction)
    - [À propos des diagrammes de classe](#a-propos-des-diagrammes-de-classe)
- [Contribution](#contribution)

## Introduction

Comme tous les domaines des mathématiques, l’analyse complexe contient entre autres de nombreux concepts.  
Les comprendre de façon séparée est une chose ; avoir une vision globale des liens entre eux et de la structure résultante en est une autre.  
Cette seconde étape n’est pas toujours évidente à atteindre, notamment car (*i*) les concepts en jeux ne sont pas triviaux, (*ii*) leur dénominations n’est pas toujours intuitive (fonction holomorphe, théorème de Cauchy, …), (*iii*) les liens entre eux ne sont pas toujours explicitement décrit, (*iv*) …  
Or, l’atteinte d’une vision d’ensemble est très bénéfique puisqu’elle facilite la mémorisation des concepts (on retient mieux plusieurs concepts si on connait leurs liens plutôt qu’en tant qu’entités individuelles et indépendantes) ainsi que le raisonnement (pour les mêmes raisons).  
Et pour ça, rien ne vaut un diagramme avec plein de cases et des flèches de partout !

<!--
Exportation PDF vers PNG :
- dimensions du PDF : 41.2 × 29.32 cm
- largeur voulue de l’image PNG : 800 px
- résolution (dpi) : 800 px / (41.2 cm / 2.54 in/cm) = 49.320388 px/in ≈ 50 dpi
-->

<p align="center">
  <img
    src="https://github.com/LaurentValade/taxonomie-analyse-complexe/blob/main/README/taxonomie-analyse-complexe.ipe.pdf.v0.0.300dpi.png"
    width="800"
    alt="Taxonomie d’analyse complexe"
  />
</p>

### À propos des diagrammes de classe

Le tier gauche de ce poster est un diagramme d’ensemble inspiré des [diagrammes de classes](https://fr.wikipedia.org/wiki/Diagramme_de_classes) de la [programmation orientée objets](https://fr.wikipedia.org/wiki/Programmation_orient%C3%A9e_objet), cette inspiration est pertinente car il y a une forte analogie entre [inclusion](https://fr.wikipedia.org/wiki/Inclusion_%28math%C3%A9matiques%29) et [héritage](https://fr.wikipedia.org/wiki/H%C3%A9ritage_%28informatique%29) :

|                        Héritage de classes                        |              Inclusion d’ensembles             |
|:-----------------------------------------------------------------:|:----------------------------------------------:|
|                    `A <- B` : `B` hérite de `A`                   |              `A <- B` : *A* ⊃ *B*              |
|           `b = B()` possède les attributs de `A` et `B`           | *B* ∋ *b* possède les propriétés de *A* et *B* |
| Il y a moins de trucs représentés par `B` que `A`<sup>**1**</sup> |           *B* est plus petit que *A*           |

[**1**]: Par exemple avec `Vehicules <- Train`, il existe moins de trains que de véhicules.

La notion importante et commune est que si `A <- B`, alors `B` possède plus de propriétés/attributs que `A` ; et par conséquent représente une population/ensemble/… plus petit.

## Contribution

J’ai réalisé ce diagramme avec l’excellent logiciel [IPE](https://ipe.otfried.org/) (développé intégralement en C++ par *Otfried Cheong*, [otfried/ipe](https://github.com/otfried/ipe)).  
En gros, c’est un *Inkscape* léger et modal, il gère nativement le LaTeX et est idoine pour ce genre de diagrammes.

Tout commentaire, proposition d’amélioration, ajout, etc. est bienvenu 🤓 !
