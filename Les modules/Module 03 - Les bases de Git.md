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
    -Le répertoire n’existe pas :
    ```
    git init <nom_répertoire>
    ```
