# Introduction

Les méthodes directes souffrent d’une capacité limitée de parallélisation et l’utilisation d’un algorithme direct avec pivot peut coûter cher en temps de calcul lorsque la taille de la matrice devient trop grande et en particulier lorsque l’on s’oriente vers des problèmes résultant de la discrétisation d’EDP en dimension 3. Lorsque la taille de la matrice augmente, les matrices sont bien creuses mais le stockage associé à la décomposition LU devient très élevé alors que le conditionnement n’est pas forcément très grand comme le montre [ce notebook](limite_direct.ipynb).

Des méthodes itératives existent depuis longtemps introduites par Jacobi et Gauss (ainsi que Ludwig von Seidel) mais certaines peuvent converger lentement. Les méthodes itératives sont revenues au goût du jour pour pouvoir attaquer des problèmes de grande taille et en particulier dans le cadre du calcul haute performance pour des matrices creuses et les problèmes réalistes actuels. Par contre, nous disposons de moins de résultats théoriques que pour les méthodes directes et l’expérimentation numérique est ici importante.