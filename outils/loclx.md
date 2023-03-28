# Outils : LocalXPose

## Description

Exposer en ligne son localhost.

## 1. Installation

Installer la version de votre système : https://localxpose.io/
(Linux 64-bit pour ce tuto)

Puis dézipper le téléchargement

```bash
unzip loclx-linux-amd64.zip
```

## 2. S'authentifier

```bash
./loclx account login
# entrer le jeton d'authentification obtenu à la création d'un compte sur leur site
```

## 3. Exposer son localhost

```bash
# --rate-limit : limiter le nombres de requêtes/m à 10 (anti DDOS)
# --https-redirect : ne pas utiliser le protocol HTTP
# --to : choisir le port à exposer
# --region : mettre votre région afin de limiter le temps de réponse du serveur
./loclx tunnel http --rate-limit 10 --https-redirect --to 127.0.0.1:3000 --region eu
```
