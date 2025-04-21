# Charnière pivot conique emboitable
_Dernière modification: 21/04/2025_

## Représentation simplifiée

<img src="../snap-clip-simple.png" class="picture" alt="Représentation simplifiée">

Contrairement aux charnières avec un pivot cylindrique, ce type de charnière peut être plus mince. Ceci est surtout dû à l'espace nécessaire pour les optimisations des charnières à pivot cylindrique.
Dans la version où l'axe est imprimé horizontalement, les deux parties peuvent se désassembler sans endommager la charnière.


<img src="../snap-clip-size.png" class="picture" alt="Dimensions de la charnière">

## Analyse de l'orientation d'impression
Imprimer l'axe de rotation horizontalement permet aux pattes d'être moins fragiles et de supporter une déformation élastique plus importante. On remarque dans le test de résistance que la version où l'axe est imprimé verticalement a moins de jeu et casse sans se désolidariser.

## Evaluation qualitative de la résistance aux contraintes
### Test de traction
| Orientation                       | Rupture | 
| --------------------------------- | -----|
| Orientation horizontale de l'axe (jeu 0.3mm)  | N/A* |
| Orientation verticale de l'axe (jeu 0.3mm) | 143 N  |
* Imprimé horizontalement, la charnière se désolidarise à 35N mais le mécanisme ne présente pas de dommage et peut être remis en place.

Photo de rupture de la charnière imprimée verticalement sous 143 N de contrainte.

<img src="../snap-clip-vertical-143N-rupture.png" class="picture" alt="Rupture orientation verticale sous 143N">

## Spécifications de jeu
| Orientation                       | Jeu  | Résultats expérimentaux           |
| --------------------------------- | -----| ------------------ |
| Orientation horizontale de l'axe  | 0.3  | Jeu libre |
| Orientation verticale de l'axe  | 0.3  | Friction moyenne* |
* la charnière ne change pas de position sous l'effet de la gravité.

<img src="../snap-clip-jeu.png" class="picture" alt="Orientation horizontale">

## Paramètres d'impression

| Différentes impressions           | Imprimante             | Filament      | Profil           | Remplissage |
| --------------------------------- | ---------------------- | ------------- | ------------- | --------- |
| Orientation horizontale de l'axe  | MK4 input shaper 0.4mm | Prusament PLA | 0.20mm Speed  | 15% |
| Orientation verticale de l'axe  | MK4 input shaper 0.4mm | Prusament PLA | 0.20mm Speed  | 15% |

## Conseils d'optimisation de conception
Aucun conseil d'optimisation, il semble que ce type de charnière soit bien adapté pour l'impression 3D.

## Citations - Sources - Attribution
Vu sur la chaine Youtube de MakerMuse [[Youtube](https://youtu.be/fbY7xHGaeNM?si=pbwtnPVgYeoj8QsR&t=240)]
