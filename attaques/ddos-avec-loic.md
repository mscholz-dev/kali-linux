# DDOS avec LOIC : Low Orbit Ion Cannon

## Description

Permet de DDOS une cible.

## 1. Installation de mono

```bash
apt install mono-complete
```

## 2. Installation de LOIC

Installer LOIC à cette URL : https://sourceforge.net/projects/loic/

Noter que la détéction de malware n'est qu'une mesure de sécurité, en aucun cas LOIC n'endommagera votre système.

## 3. [optionnel] Installation de nload

```bash
apt install nload
```

## 4. Lancer LOIC

```bash
# depuis le dossier où se trouve le zip :
unzip LOIC-1.0.8-binary.zip

# exécuter LOIC
mono LOIC.exe
```

## 5. [optionnel] Lancer nload

nload permet de voir le traffic réseau pour mieux visualiser l'attaque DDOS, lancer cette commande dans un second terminal, en même temps que LOIC.

```bash
nload
```

## 6. [optionnel] Créer un serveur ExpressJS afin de le DDOS en local

### 1. Mise en place du serveur ExpressJS

```bash
# créer un dossier pour le serveur ExpressJS
mkdir express-server-hack

# se mettre dans le dossier créé
cd express-server-hack

# initier npm (nécessite npm sur le système)
npm init -y

# installer ExpressJS
npm i express

# installer nodemon pour relancer le serveur automatiquement en cas de changement dans le code
npm i nodemon

# créer le serveur ExpressJS
nano app.js
```

```js
// ajouter ce code dans app.js
const express = require("express");
const app = express();
const port = 3000;

// stocker le nombre de requêtes reçues
let requested = 0;

// route: 127.0.0.1:3000 (ou localhost:3000)
app.get("/", (req, res) => {
  // incrémenter le nombre de requêtes reçues
  requested++;

  // afficher la valeur dans le terminal
  console.log(requested);

  res.send("Hello World!");
});

app.listen(port, () => {
  console.log(`ExpressJS app listening on port ${port}`);
});
```

```bash
# modifier le script de démarrage du serveur
nano package.json

# mettre ce code à la place du "scripts" existant
```

```js
"scripts": {
    "start": "nodemon app.js"
  },
```

```bash
# lancer le serveur ExpressJS
npm start
```

Pour vérifier que le serveur fonctionne, rendez-vous sur l'URL : http://127.0.0.1:3000/

Si le message "Hello World!" apparaît sur votre navigateur, le serveur est prêt!

### 2. DDOS notre serveur ExpressJS

Dans LOIC, renseigner :

- IP : 127.0.0.1
- PORT : 3000
- METHODE : HTTP

Il ne reste plus qu'à lancer l'attaque sur le serveur ExpressJS avec le bouton "IMMA CHARGING MAH LAZER".

Si toutes les étapes précédentes sont respecté, dans le terminal tournant le serveur ExpressJS, vous y verrez des milliers de requêtes faite, l'attaque DDOS est en cours!
