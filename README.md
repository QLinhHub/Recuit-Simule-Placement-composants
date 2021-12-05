# Recuit-Simule-Placement-composants

Le probléme consiste à trouver la configuration optimale de connexion entre différents blocs d’un
circuit integré. C’est un problème d’optimisation difficile nécessitant l’utilisation de métaheuristiques
pour trouver une solution approchée. Lors d’une application réel les temps de calculs sont très
elevés vu le grand nombre d’éléments à traiter.

Dans notre cas les blocs sont disposés de facon regulière sur une grille carrée. La fonction
coût est calculée en effectuant la somme des coûts de chaque connexion. Le coût d’une connexion
est égal à la distance de Manhattan entre les deux blocs de cette connexion. Pour ce problème,
la distance entre deux blocs est fixée à 5. Ainsi, pour une grille de taille 5 × 5, la valeur optimale
est de 200.

Ce problème se prête bien à une résolution par recuit simulé. Nous effectuons une ini-
tialisation aléatoire de la grille puis nous appliquons l’algorithme vu précedemment. Le seul
mouvement élémentaire disponible est la la permutation des positions de 2 blocs de la grille.
Les blocs à permuter sont choisis aléatoirement à chaque étape du recuit simulé.

Ce problème est aussi appelé Placement-Routage (Place and Route).
