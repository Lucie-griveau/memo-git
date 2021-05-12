# memo-git
Synchroniser un répo sur GitHub avec commande en local (git bash)
    - git remote add origin <lien HTTP ou SSH dispo dans GitHub>
    - git push -u origin master (ou main en fonction de la branch)

Versionner ses fichiers
    - cd <chemin du dossier> (attention /g/ et pas \g\)
    - git init (une seule fois)
    - git add . (ajoute tous les fichiers du dossier)
    - git status (pour voir l'état des fichiers, à répérer si besoin ou problèmes)
    - git commit -m "commentaires" (faire un commentaire précis)
    - git add puis git commit (si modification(s) apportée(s) sur un fichier)
    - git log (une seule fois pour voir tous les commit)
    - git push (une seule fois pour tous les commits ou après chaque commit)

Utiliser la ligne de commande (git bash)
    - pwd = dans quel répertoire on se trouve
    - ls = quels sont les fichiers dans ce répertoire
    - ls -al = idem ls mais avec les fichiers en cache

Gérer un conflit
    - git status
    - supprimer la ligne conflictuelle dans VSCode (vert = local, bleu = distance)
    
<<<<<<< HEAD
open an issue
=======
ask your question in IRC.
>>>>>>> branch-a

    - git add
    - git commit -m "fixed merge conflict"