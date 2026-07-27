### Navigation dans les Répertoires..
- `cd <répertoire>` : Aller dans le répertoire spécifié.
- `cd ..` : Revenir au répertoire parent.
- `pwd` : Afficher le chemin du répertoire courant.

### Lister les Fichiers
- `ls` : Lister les fichiers dans le répertoire courant.
- `ls -l` : Lister les fichiers avec détails (permissions, propriétaire, taille, etc.).
- `ls -a` : Lister tous les fichiers, y compris les fichiers cachés.

### Gestion des Fichiers et Répertoires
- `mkdir <répertoire>` : Créer un nouveau répertoire.
- `touch <fichier>` : Créer un nouveau fichier vide.
- `cp <source> <destination>` : Copier un fichier ou un répertoire.
- `mv <source> <destination>` : Déplacer ou renommer un fichier ou un répertoire.
- `rm <fichier>` : Supprimer un fichier.
- `rm -r <répertoire>` : Supprimer un répertoire et son contenu.

### Affichage du Contenu des Fichiers
- `cat <fichier>` : Afficher le contenu d'un fichier.
- `less <fichier>` : Afficher le contenu d'un fichier page par page.
- `head <fichier>` : Afficher les premières lignes d'un fichier.
- `tail <fichier>` : Afficher les dernières lignes d'un fichier.

### Gestion des Processus
- `ps` : Afficher les processus en cours.
- `top` : Afficher en temps réel les processus les plus consommateurs de ressources.
- `kill <PID>` : Terminer un processus en utilisant son PID.

### Gestion des Permissions
- `chmod +x <fichier>` : Rendre un fichier exécutable.
- `chmod 755 <fichier>` : Changer les permissions d'un fichier ou d'un répertoire.

### Commandes Réseau
- `ping <adresse>` : Vérifier la connectivité réseau avec une adresse IP ou un nom de domaine.
- `curl <URL>` : Télécharger le contenu d'une URL.
- `wget <URL>` : Télécharger un fichier depuis une URL.

### Compression et Décompression
- `tar -czvf <archive.tar.gz> <répertoire>` : Compresser un répertoire en archive `.tar.gz`.
- `tar -xzvf <archive.tar.gz>` : Décompresser une archive `.tar.gz`.

### Utilisation de Git
- `git status` : Vérifier l'état du dépôt Git.
- `git add <fichier>` : Ajouter un fichier à l'index pour le prochain commit.
- `git commit -m "message"` : Créer un commit avec un message descriptif.
- `git push` : Pousser les commits locaux vers le dépôt distant.

### Redirection d'Entrée/Sortie
- `echo "Texte" > <fichier>` : Écrire du texte dans un fichier (écrase le contenu existant).
- `echo "Texte" >> <fichier>` : Ajouter du texte à la fin d'un fichier (sans écraser le contenu existant).
# public_test# public_test


# Le repertoire sert à connaitre les bases de GitHub

# Commandes Git

## Commandes de Base

### Configuration Initiale
- `git config --global user.name "Ton Nom"` : Définit ton nom d'utilisateur.
- `git config --global user.email "ton.email@example.com"` : Définit ton adresse e-mail.

### Gestion des Dépôts
- `git init` : Initialise un nouveau dépôt Git dans le répertoire actuel.
- `git clone <URL>` : Clone un dépôt distant sur ta machine locale.

### États et Informations
- `git status` : Affiche l'état des fichiers dans le répertoire de travail.
- `git log` : Affiche l'historique des commits.
- `git diff` : Montre les différences entre les fichiers modifiés et les fichiers dans l'index.

### Gestion des Fichiers
- `git add <fichier>` : Ajoute des fichiers spécifiques à l'index (prépare les fichiers pour le commit).
- `git add .` : Ajoute tous les fichiers modifiés et nouveaux à l'index.
- `git rm <fichier>` : Supprime des fichiers du répertoire de travail et de l'index.

### Commits
- `git commit -m "Message"` : Crée un commit avec un message descriptif.
- `git commit --amend` : Modifie le dernier commit (ajoute des changements ou change le message).

### Pousser et Tirer
- `git push origin <branche>` : Envoie les commits de ta branche locale vers la branche distante spécifiée.
- `git pull origin <branche>` : Récupère les changements de la branche distante et les fusionne avec ta branche locale.

### Gestion des Branches
- `git branch` : Liste les branches locales.
- `git branch <nom>` : Crée une nouvelle branche.
- `git checkout <nom>` : Change de branche.
- `git checkout -b <nom>` : Crée une nouvelle branche et change pour cette branche.
- `git merge <branche>` : Fusionne une branche avec la branche actuelle.
- `git branch -d <nom>` : Supprime une branche locale.

### Gestion des Dépôts Distants
- `git remote -v` : Affiche les dépôts distants configurés.
- `git remote add <nom> <URL>` : Ajoute un nouveau dépôt distant.
- `git remote remove <nom>` : Supprime un dépôt distant.

### Réinitialisation et Rebasage
- `git reset <fichier>` : Annule les modifications dans un fichier depuis le dernier commit.
- `git reset --hard <commit>` : Réinitialise le dépôt au commit spécifié (attention, cela supprime les changements non commités).
- `git rebase <branche>` : Rebase la branche actuelle sur une autre branche (utile pour réécrire l'historique).

## Commandes Avancées

### Gestion des Tags
- `git tag` : Liste les tags.
- `git tag <nom>` : Crée un tag.

### Gestion des Conflits
- `git status` : Utile pour identifier les fichiers en conflit.
- `git mergetool` : Lance un outil de fusion pour résoudre les conflits.

### Stashing
- `git stash` : Met de côté les modifications non commités.
- `git stash pop` : Récupère les modifications mises de côté avec `git stash`.

### Rechercher
- `git grep <motif>` : Recherche un motif dans les fichiers du dépôt.

