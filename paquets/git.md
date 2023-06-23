# Ajout de paquet : git

[↩️ Retour](./README.md)

## Description

Permet la gestion de versions.

## 1. Installation

```bash
apt install git
```

## 2. Authentification de git

```bash
git config --global user.name [NOM]
git config --global user.email [EMAIL]

# main comme nom de branche par défaut
git config --global init.defaultBranch main

# en cas de conflit, merge par défaut
git config --global pull.rebase false

# changer checkout en co (alias)
git config --global alias.co checkout
```
