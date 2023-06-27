# Mes aliases

[↩️ Retour](./README.md)

## 1. Modifier le fichier .zshrc

```bash
nano ~/.zshrc
```

## 2. Ajouter les aliases à la fin du fichier

```bash
# nettoyer la console
alias c="clear"

# accès rapide aux dépôts github
alias projects="~/Documents/projects"

# lancer vscode
alias code="snap run code"

# accès rapide aux outils (hacking)
alias tools="~/Documents/tools"

# lancer mechvibes sans recevoir ou tenir le terminal (changer le chemin)
alias tws="cd ~ && setsid ./Documents/tools/mechvibes/opt/Mechvibes/mechvibes &>/dev/null"

# lancer postman sans recevoir ou tenir le terminal
alias postman="setsid snap run postman &>/dev/null"

```

## 3. Mettre à jour les aliases du fichier .zshrc

```bash
source ~/.zshrc
```
