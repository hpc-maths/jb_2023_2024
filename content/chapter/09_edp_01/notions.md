# Notions essentielles

Dans cette section, nous focalisons notre attention sur l’équation de la chaleur, une équation scalaire linéaire, dans un premier temps et abordons ensuite son pendant non-linéaire en ajoutant un terme source non-linéaire pour obtenir une équation de réaction-diffusion dite de Nagumo, qui admet des solutions de type ondes progressives.

Dans un [premier notebook](./heat_edo.ipynb), nous considérons un ensemble de méthodes numériques en temps d’ordre un et deux, explicites et implicites pour résoudre l'équation de la chaleur et faisons le lien entre solution fondamentale exacte, solution quasi-exacte pour une discrétisation spatial fixée et solution numérique de l’EDP sur un intervalle de temps et d’espace. Les ordres de convergence obtenus par la théorie sont retrouvés expérimentalement.

Dans un [deuxième notebook](./vp_laplacien.ipynb), la notion de raideur du système d’EDO obtenu précédemment est analysée graphiquement (théoriquement dans le cours) sur la base du spectre de l’opérateur de Laplace continue et de sa discrétisation spatiale par différences finies. On retrouve le conditionnement de la matrice de discrétisation du Laplacien en $1/\delta x_2$ en lien direct avec la raideur modérée sur système.

Dans un [troisième notebook](./heat_edp.ipynb), nous considérerons la notion de convergence au sens des EDPs dans la lignée de la théorie de Lax et Richtmyer. Il y a ici quelques subtilités suivant comment on lie le pas d’espace et de temps, en particulier lorsque l’on a la latitude de les choisir indépendamment dans le cadre de méthodes implicites.

Enfin, Nous terminons par une [résolution avec diverses méthodes numériques de l’équation de Nagumo](./nagumo.ipynb) (Splitting, IMEX). Il s’agit d’un cas d’école de résolution d’une équation non-linéaire et permet de saisir l’étendues des techniques possibles pour aborder ce type d’équation.