# Module 03 - Les bases de Git
- Le dépôt
    - Création d’un dépôt local.
- Travailler avec le dépôt
    - Publier des fichiers.
    - Enregistrer des modifications.
    - Visualiser l’historique.
    - Annuler des actions.

# Dossier de travail vs. Dépôt Git
- Le dossier de travail :
    - Il contient les fichiers du projet.
    - Il peut exister avant une prise en charge par Git.
    - Il est local sur le poste de travail du développeur.
- Le dépôt Git :
    - Il contient tout l’historique du projet, toutes les modifications, toutes les 
révisions…
    - C’est le dossier .git du dossier de travail 

# Le dépôt Git
- Un dépôt Git est un répertoire contenant l’historique d’un projet logiciel.
- Un dépôt local :
    - Est situé sur la machine du développeur ;
    - N’est pas partagé entre plusieurs développeurs.
- Pour créer un dépôt, il faut initialiser un répertoire avec la structure 
nécessaire.
- Deux cas de figure : 
- Le répertoire existe déjà (et contient peut être des fichiers de projet !) :
    - Se positionner dans le répertoire 
    ```
    git init
    ```
    - Le répertoire n’existe pas :
    ```
    git init <nom_répertoire>
    ```

# Ajout de fichiers au dépôt
- Pour qu’un fichier passe sous contrôle de version Git, il faut d’abord l’ajouter 
au dépôt.
- Commande git add
    - Elle va ajouter le(s) fichiers dans la zone d’index, ils sont simplement marqués et ne 
sont pas encore ajoutés !
- Ajouter un fichier :
```
git add test.js
```
- Ajouter tous les fichiers du répertoire :
```
git add .
```
- Ajouter de manière interactive :
```
git add -p
```
- A tout moment, la commande git status permet de connaître l’état du dépôt Git ! 

# Valider des fichiers dans le dépôt
- Valider les fichiers dans le dépôt consiste à envoyer les fichiers présents dans la 
zone d’index dans le dépôt.
    - C’est le « commit » !
    - Chaque commit concerne une collection de modifications apportées à un ou 
plusieurs fichiers.
- Pour le bon suivi de l’historique du projet, chaque commit doit être associé à un 
message décrivant les modifications qui sont apportées au projet par cette 
validation.
- Validation avec ouverture de l’éditeur de texte pour la saisie du message : 

```
git commit
```

- Validation avec message : 

```
git commit -m "Mon commentaire constructif"
```

- Indexation et commit en une seule commande ! : 
  
```
git commit -am "Mon commentaire constructif"
```
  
- Cela permet d’enregistrer toutes les modifications en cours, même celles non-indexées ! 
- ATTENTION : Cela ne s’applique qu’aux fichiers déjà existant dans le dépôt
 
# git commit : Bonnes pratiques

- Bonne pratique de « commit » Git :
    - Ne concerne qu’une seule fonctionnalité du projet ;
    - Est le plus petit possible tout en restant cohérent ;
    - Idéalement, compile seul.
- Un commit n’est pas, contrairement aux idées reçues, une liste 
d’ajout/suppression/modification de lignes !
    - Git sauvegarde chaque fichier entièrement à chaque changement.
        - Avec des métadonnées (commentaire, auteur, email, date, …)

# Etats de fichiers
- La commande git status permet de lister les modifications en cours du 
dossier de travail et de la zone d’index.
- En gros, les fichiers non enregistrés dans le dépôt.
- Quatre états possibles :
- **untracked**
    - Non suivi, le fichier est inconnu de Git !
- **unmodified**
    - Le fichier n’a pas été modifié depuis son dernier ajout au dépôt.
- **modified**
    - Il y a des différences entre le fichier du répertoire de travail et celui du dépôt.
- **staged**
    - Le fichier est dans la zone d’index, il sera ajouté au prochain commit.
