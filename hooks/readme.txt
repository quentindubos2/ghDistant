
INSTALLATION DU HOOK PRE-COMMIT

Objectif :
Ce hook permet d'enregistrer automatiquement la date
et l'heure de verification d'un commit.

Installation :
1. Cloner le depot Git.
2. Copier le fichier hooks/pre-commit dans .git/hooks/.
3. Conserver le nom pre-commit sans extension.

Commande PowerShell :
Copy-Item hooks/pre-commit .git/hooks/pre-commit

Fonctionnement :
Lors d'un git commit, le hook demande une confirmation.

- y : cree ou met a jour suivi/commitInfo.txt
      et ajoute le fichier au commit.
- n : poursuit le commit sans modifier le fichier.
- Entree : meme comportement que n.

Remarque :
Les hooks Git ne sont pas partages automatiquement.
Chaque developpeur doit installer le hook localement.