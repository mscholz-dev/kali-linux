# Fonctionnalité : bruit de clavier audio

## Description

Permet de jouer des sons personnalisés à chaque frappe de touche.

## 1. Installer l'exécutable

Se rendre sur ce lien : https://github.com/hainguyents13/mechvibes

## 2. Extraire l'exécutable dans le dossier "tools"

```bash
cd Téléchargement
mkdir ~/Documents/tools/mechvibes
mv mechvibes_2.3.0_amd64.deb ~/Documents/tools/mechvibes/mechvibes_2.3.0_amd64.deb
cd ~/Documents/tools/mechvibes
dpkg-deb -xv mechvibes_2.3.0_amd64.deb .
```

## 3. Exécuter mechvibes

```bash
./opt/Mechvibes/mechvibes
```

## 4. Ajouter un alias pour l'exécuter

[Voir les aliases](../aliases.md)
