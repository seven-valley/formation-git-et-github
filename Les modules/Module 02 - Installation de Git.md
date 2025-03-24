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