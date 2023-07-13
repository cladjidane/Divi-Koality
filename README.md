# Divi-Koality
Thème enfant de Divi by Koality!

***
***Ce thème est une base minimal***

Voir les autres thèmes de base :
* Avec Tailwind (***TODO***)
* Avec Gulp (***TODO***)

***

## Téléchargement

Directement via github

Via CLI

```wget https://github.com/cladjidane/Divi-Koality/archive/refs/heads/main.zip ; unzip main.zip ; rm main.zip```

## Installation de Tailwind

Sous plesk, executer npm via : 
```export PATH=$PATH:/opt/plesk/node/20/bin/```
(J'aimerais résoudre ce probleme sou sPLESK !!)

Puis executer pour initilaiser le package.json :
```npm init```

Installer ensuite Tailwind : 
```npm install -D tailwindcss```

Initialiser tailwindcss :
```npx tailwindcss init``` 

Spécifier les fichiers à surveiller :
```
module.exports = {
  content: ["./**/*.php"],
  theme: {
    extend: {},
  },
  plugins: [],
}
``` 

Puis lancer le watcher pour surveiller les modifications sur les fichiers
```npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch```

## Modifications à faire :

* Changer le nom du dossier (supprimer - main)
* Changer dans style.css "_CLIENT_" ligne 5 "Description:  Thème enfant de Divi pour _CLIENT_ by Koality!"
