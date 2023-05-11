# Ajout de paquet : discord

[↩️ Retour](./README.md)

## Description

installer discord via le site officiel sinon l'extension "rich presence" ne marchera pas (pas depuis snap ni flatpak).

## 1. Installation

Télécharger le paquet à l'URL suivante : https://discord.com/download

```bash
# dans le dossier téléchargement
dpkg -i discord*.deb
```

## 2. Finir l'installation

```bash
apt install --fix-broken
```

## 3. Lancer l'application

Elle se trouve avec la barre de recherche du système d'exploitation en écrivant : Discord

Ou avec le terminal

```bash
discord
```
