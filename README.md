Arena de Défis Algorithmiques

Plateforme C Interactive de Competitive Programming

Arena de Défis est une application entièrement développée en langage C, proposant plusieurs mini-jeux algorithmiques pour entraîner les étudiants à la résolution de problèmes, à l’optimisation et à la pensée computationnelle.
Le système inclut un tableau de bord animé, des défis progressifs, un historique, un classement global et un système de scoring.


le Projet est réalisé à l’École Nationale des Sciences de l’Informatique (ENSI) par les élèves :
Askri Isra
Elaa Ben Aoun
Riahi Dalia


📌 Fonctionnalités Principales
🔹 1. Défi : Countdown (Le Compte est Bon)

Implémenté dans countdown.c

Génération aléatoire de 6 nombres

Création d'un objectif solvable via un moteur d’opérations internes

Résolution étape par étape avec opérations : + - * /

Système de réinitialisation (Reset)

Ajout automatique de 50 points en cas de réussite

🔹 2. Défi : Mastermind Algorithmique

Implémenté dans tache2proj.c

Une séquence secrète est générée

Le joueur propose une combinaison

Le système répond :

✔️ bons chiffres bien placés

❌ bons chiffres mais mal placés

Score attribué selon performance

🔹 3. Défi : Robot Maze

Implémenté dans ROBOTMAZE.c

Exploration d’un labyrinthe sous forme de grille

Algorithme de recherche du chemin le plus court

Visualisation du parcours

Attribution de points selon le temps/chemin trouvé

🔹 4. Défi : Tri Ultime (Ultimate Sort)

Implémenté dans TRIULTIMATE.c

Défis de tri avec contraintes

Comptage des opérations effectuées

Score selon efficacité de l’algorithme

🔹 5. Système de Score, Historique & Classement

Implémenté dans leaderboard.c

Fichier utilisé : history_log.txt

Sauvegarde automatique :

nom du joueur

mission réalisée

points gagnés

Classement global trié décroissant

Journal personnel du joueur

🔹 6. Interface Utilisateur Interactive

Implémenté dans interface.c

Menu coloré en ASCII Art

Authentification du joueur

Tableau de bord dynamique

Navigation vers les différents défis

Système de rangs :

Newbie (0–50 pts)

Intermédiaire (51–100 pts)

Expert (100+ pts)

🗂️ Structure du Projet
/Arena-De-Defis
│── interface.c
│── countdown.c
│── tache2proj.c
│── ROBOTMAZE.c
│── TRIULTIMATE.c
│── leaderboard.c
│── history_log.txt       (généré automatiquement)
│── README.md


🛠️ Compilation & Exécution
✔️ Compilation (simple)
gcc interface.c -o arena


⚠️ Assurez-vous que tous les fichiers .c sont dans le même dossier,
car interface.c les inclut directement via :

#include "countdown.c"
#include "tache2proj.c"
#include "leaderboard.c"
#include "ROBOTMAZE.c"
#include "TRIULTIMATE.c"

▶️ Lancer le programme
./arena

📊 Système de Points
Défi	Points typiques
Countdown	+50 pts
Mastermind	variable
Robot Maze	+50 pts
Ultimate Sort	+20 pts
Bonus / variantes	selon mission

Un historique complet est conservé dans history_log.txt.

🧪 Exemple de Session

L'utilisateur entre son nom

Accède au menu coloré

Lance un défi

Gagne un score → automatiquement enregistré

Le classement global se met à jour
