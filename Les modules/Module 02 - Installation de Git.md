# Module 02 - Installation de Git

- Principes d’installation selon le système d’exploitation
    - Installation sous Linux
    - Installation sous macOS
    - Installation sous Windows
- Validation de l’installation et premières commandes
    - L’aide en ligne de commande
    - Principes et syntaxe des commandes Git
- Configuration post-installation
    - Création de comptes d’utilisateur

## Installation de Git
- Installation sous Linux
    - A partir de paquets existants dans la distribution.
    - A partir des sources.
- Installation sous macOS
    - Avec Homebrew
    - Avec XCode
- Installation sous Windows
    - Avec un installeur

## Installation sous Linux
- A partir des paquets d’une distribution
    - RedHat, CentOS, Fedora
        - sudo yum install git
    - Debian, Ubuntu
        - sudo apt install git
- A partir des sources
    - Installation des dépendances
        - _make, libssl-dev, libz-dev, gettext, libexpat1-dev, libcurl4-openssl-dev, build-essential_
    - Récupération et décompression du code source de Git
        - https://github.com/git/git/archive/v2.27.0.tar.gz
- Compilation et installation
    - cd code_git/git-2.27.0 
    - make prefix=/usr/local all 
    - make prefix=/usr/local install

## Installation sous macOS
- Git est fourni avec l’IDE XCode
    - Aucune installation supplémentaire nécessaire.
- _Command Line Tools for XCode_ permet d’installer   les outils de 
développement en ligne de commande (dont Git !) sans avoir besoin 
d’installer tout XCode.
    - Apple Developer ID nécessaire !
- Avec Homebrew
    - Télécharger et installer Homebrew (Un     gestionnaire de paquets pour macOS)
        - https://brew.sh
    - Dans un terminal
        - brew install git

## Installation sous Windows
 - Un installeur graphique est disponible
    - https://git-scm.com/download/win
-Il installe : 
    - Une intégration à l’explorateur Windows
    - Git Bash, permettant de disposer du shell Bash sous Windows
        - Et donc de certaines commandes Linux.
    - Un gestionnaire de mots de passe
    - Permettant de mémoriser les authentifications aux différents dépôts

 <img src="./img/02-git-bash.png" width="600">
 
## La ligne de commande
- Git s’utilise en ligne de commande !
    - Terminal Linux ou macOS
    - Git Bash sous Windows (recommandé) ou une simple Invite de commande
- Syntaxe :
    - git <commande> [<arguments>]

    <img src="./img/02-git-commande.png" width="600">
```
git --version
```