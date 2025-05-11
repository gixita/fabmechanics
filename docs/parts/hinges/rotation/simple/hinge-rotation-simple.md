# Charnière universelle simple et détachable
_Dernière modification: 21/04/2025_

## Représentation simplifiée
![Dessin d'une charnière universelle simple et détachable](./hinge-rotation-simple.png)

[Modèle FreeCad avec optimisation de conception](./hinge-rotation-simple-toprint.FCStd)

## Analyse de l'orientation d'impression
### Orientation horizontale de l'axe de rotation
__Avantages__ : Résistance plus élevée à la [traction](../effort-traction.png) et la [flexion](../effort-flexion.png).

__Inconvénients__ : Lignes de couche visibles sur les surfaces courbes, les tolérances sont moins précises.

<img src="../Orientation-horizontale.png" width="400" alt="Orientation horizontale">

### Orientation verticale de l'axe de rotation
__Avantages__ : Surfaces de rotation plus lisses.

__Inconvénients__ : Risque de délamination des couches sous charge.

<img src="../Orientation-verticale.png" width="400" alt="orientation verticale">

<!-- 
## Evaluation qualitative de la résistance aux contraintes

| Orientation                       | Effort 1          | Effort 2           |
| --------------------------------- | ----------------- | ------------------ |
| Orientation verticale de l'axe    | Résistance faible | Résistance faible  |
| Orientation horizontale de l'axe  | Resistance haute  | Resistance moyenne |

-->
## Spécifications de jeu
| Orientation                       | Jeu          | Résultats expérimentaux           |
| --------------------------------- | ----------------- | ------------------ |
| Orientation verticale de l'axe    | 0.15 | Jeu libre  |
| Orientation horizontale de l'axe  | 0.15  | Friction moyenne |
| Orientation horizontale de l'axe  | 0.3  | Jeu libre |


## Paramètres d'impression utilisés

| Différentes impressions           | Imprimante             | Filament      | Profil           |
| --------------------------------- | ---------------------- | ------------- | ------------- |
| Orientation verticale de l'axe    | MK4 input shaper 0.4mm | Prusament PLA | 0.20mm Speed |
| Orientation horizontale de l'axe  | MK4 input shaper 0.4mm | Prusament PLA | 0.20mm Speed  |


## Conseils d'optimisation de conception
- Augmenter le diamètre de l'axe pour une plus grande résistance.
- Ajouter un méplat sur l'axe/pivot pour faciliter le pont (bridging)

<img src="../opt-meplat.png" class="picture_optimisation">

- Ajouter une pointe à l'alésage (pièce femelle) afin d'éviter un effondrement dû au porte-à-faux (overhang). De plus, la partie haute d'un trou rond va être approximée par un plat dans le slicer, ce qui peut donc diminuer localement la taille du trou.

<img src="../opt-v.png" class="picture_optimisation">

- Ajouter un chanfrein à la base du pivot augmente la résistance de la pièce. Le chanfrein du pivot devrait être plus petit que celui de l'alésage afin de minimiser la friction dans la charnière.

<img src="../opt-chanfrein.png" class="picture_optimisation">

## Citations - Sources - Attribution
Pas d'application
