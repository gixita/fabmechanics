# Trou adaptatif vu sur Slant3D.

Ce trou adaptatif est particulièrement efficace car il permet de garder l'alésage aligné sur son axe, ce qui n'est pas le cas de toutes les solutions de trou adaptatif.

Nous avons réalisé plusieurs essais afin de déterminer comment dessiner ce type de trou.

Lors d'une impression d'un cylindre de 20mm, le diamètre mesuré était de 19.8mm, ce qui implique que le trou doit accomoder des erreurs au minimum de 0.2mm dans les deux directions.
Or nous avons besoin que le système se déforme afin un tight fit. 

Si le design des dents est trop grossier, la déformation élastique sera trop faible, plus les dents seront fines plus elles pourront se déformer élastiquement. Par contre, des dents trop fines peut également poser problème. Le rayon de l'extrémité de la dent doit être au moins de 0.4m avec une buse de 0.4mm car sinon l'extrémité de la dent ne pourra pas être imprimée. C'est une bonne pratique ici d'analyser le résultat dans le slicer pour voir s'il est capable de créer la dent.

<img src="../TooSmallToothsP10.png" class="center">

Avantages:

- Le centre de l'axe reste aligné avec l'axe de l'alésage.
- Permet de grande variation d'erreur sur les dimensions (donc être robuste à différentes imprimantes 3D).

Inconvénients de cette technique:

- Si un effort est appliqué sur l'axe, il peut y avoir un désalignement entre l'axe et l'alésage.
- Il est impossible d'obtenir un serrage fort entre l'axe et l'alésage.
- Prends du temps à dessiner.
- Le design prend plus de place qu'un simple trou.
- Ce design n'est pas adapté pour une impression verticale.

## Dessiner un trou adaptatif à dents

- Créer un trou du diamètre + 6mm dans votre solide
- Dans un nouveau sketch, nous allons dessiner une dent qui sera extrudée et ensuite, on utilisera un polar pattern.

Pour le dessin de la dent:

- Créer un cercle de construction de diamètre du trou + 6mm
- Créer un autre cercle de construction d'un diamètre - 0.5mm
- Créer deux droites de constructions d'un angle de 15° à gauche de l'ordonnée et l'autre droite de construction à 25° à droite de l'ordonnée.
- Créer les trois arcs de cercle approximativement 
- Rejoindre les arcs de cercles à l'aide de segments de droites et ajouter les contraintes de tangeance.
- Le rayon de courbure de la pointe de la dent ne devrait pas être plus petit que la taille de la buse sinon le slicer devra restreindre la longueur de la dent. Votre trou sera alors plus grand que prévu.
- Il est ici intéressant de vérifier dans le slicer que tout est conforme à votre design.

<img src="../sketch_adaptaive_slant_hole.png" class="center">
