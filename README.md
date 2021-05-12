# memo-git
Synchroniser un répo sur GitHub avec commande en local (git bash)
1) git remote add origin <lien HTTP ou SSH dispo dans GitHub>
2) git push -u origin master (ou main en fonction de la branch)

Versionner ses fichiers
1) git init (une seule fois)
2) git add . (ajoute tous les fichiers du dossier)
3) git status (pour voir l'état des fichiers, à répérer si besoin ou problèmes)
4) git commit -m "commentaires" (faire un commentaire précis)
5) git add puis git commit (si modification(s) apportée(s) sur un fichier)
6) git log (une seule fois pour voir tous les commit)
7) git push (une seule fois pour tous les commits ou après chaque commit)

Utiliser la ligne de commande (git bash)
- cd <chemin du dossier> (attention /g/ et pas \g\)
- pwd = dans quel répertoire on se trouve
- ls = quels sont les fichiers dans ce répertoire
- ls -al = idem ls mais avec les fichiers en cache

Gérer un conflit
1) git status
2) supprimer la ligne conflictuelle dans VSCode (marqueur de conflit: vert = HEAD local, bleu = distance)
<<<<<<<HEAD (Current Change)
ligne modifiée en local
=======
ligne modifiée en distant
>>>>>> branch-a (Incomming Change)
3) git add <le fichier modifier ou tout>
4) enchainer git status et git add si beaucoup de fichiers en conflit
5) git commit -m "fixed merge conflict"