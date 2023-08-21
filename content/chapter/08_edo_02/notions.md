# Notions essentielles

Dans un premier temps, nous reprenons [l’équation de Curtiss et Hirschfelder](./curtiss_rk.ipynb), qui constitue un très bon modèle jouet permettant de jouer avec la raideur du système et d’illustrer la notion de stabilité linéaire ou stabilité absolue. En particulier, nous considérons les méthodes explicites en lien avec la raideur et le diagramme de stabilité afin de voir l’impact de la raideur et de l’ordre sur les résultats.

Nous traitons ensuite [le système d’équations de Belousov et Zhabotinsky](./brusselator_rk.ipynb) (réactions chimiques oscillantes) afin d'étudier le coût calcul à précision fixée.

Pour finir, l’ensemble des méthodes sont testées sur le problème très non-linéaire de [l’explosion thermique](./explosion_rk.ipynb). Cette équation scalaire implique des valeurs propres réelles positives de très large amplitude dans un régime initial de type explosion puis des valeurs propres réelles négatives de très grande amplitude menant à une très forte raideur en fin d’intégration. Nous illustrons le fait que pour ce type de problème, la « bonne » stratégie consiste à utiliser une méthode implicite à pas de temps adaptatif d’ordre élevé, type Radau 5.
