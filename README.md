- Le README présentera le workflow Git choisi en expliquant ses avantages et/ou inconvénients

\*Branches principales :

main : Branche principale qui représente l'état de production de votre application. Les déploiements en production sont effectués à partir de cette branche.
develop : Branche de développement principal où le développement continu de nouvelles fonctionnalités a lieu. Les fonctionnalités sont fusionnées dans cette branche depuis les branches de fonctionnalités une fois qu'elles sont prêtes.

Branche de fonctionnalité :

pipeline : Branche sur laquelle la fonctionnalité actuelle est developpée. Les fonctionnalités sont développées isolément sur des branches de fonctionnalités dédiées avant d'être fusionnées dans develop.

\*Avantages :

Isolation des fonctionnalités : En développant chaque fonctionnalité sur sa propre branche (pipeline), nous isolons les changements liés à cette fonctionnalité, ce qui réduit les conflits et facilite la gestion des modifications.
Clarté dans le développement : La séparation claire des branches main, develop et pipeline permet une compréhension facile de l'état actuel du développement et des déploiements.
Stabilité de la branche principale : La branche main reste stable car elle ne reçoit que des mises à jour une fois que les fonctionnalités sont terminées et prêtes à être déployées.

\*Inconvénients :

Complexité accrue : Le modèle Gitflow peut devenir complexe à mesure que le nombre de branches augmente, ce qui peut rendre difficile la gestion des branches et des fusionnements.
Overhead de gestion : La gestion des différentes branches (notamment les branches de fonctionnalités) peut ajouter de la charge administrative.
