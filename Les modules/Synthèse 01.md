# Synthèse 01

## Les 6 commandes
- 1 Initialiser un projet git
```
git init
```

- 2 je défini la branche main
```
git branch -M main
```

- 3 je definis le depot distant (GitHub) rao
```
git remote add origin <repository>
```

- 4 Ajouter dans le staging
```
git add .
```

- 5 je fais le commit
```
git commit -m "first commit"
```

- 6 j'envoie vers le repo distant
```
git push -u origin main
```

```
git push 
```

# Scénario de Mr Pink et Mr Blue

Comment fait Mr Blue pour récupérer le repo de Mr Pink ?
```
git clone <repo>
```
:warning: attention on récupère un répertoire

Comment fait Mr Pink pour récupérer le travail de Mr Blue ?  
votre est "ahead"
```
git pull
```
