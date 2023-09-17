# Mes aliases

[↩️ Retour](./README.md)

## 1. Modifier le fichier .zshrc

```bash
nano ~/.zshrc
```

## 2. Ajouter les aliases à la fin du fichier

```bash
# (facultatif) lancer mechvibes sans recevoir ou tenir le terminal (changer le chemin)
# alias tws="cd ~ && setsid ./Documents/tools/mechvibes/opt/Mechvibes/mechvibes &>/dev/null"
alias c="clear"
alias projects="/home/ilak/Documents/projects"
alias code="snap run code"
alias postman="setsid snap run postman &>/dev/null"
alias journalstart="sudo systemctl stop systemd-journald"
alias journalrm="sudo rm -r /var/log/journal/*"
alias journalstop="sudo systemctl start systemd-journald"

```

## 3. Mettre à jour les aliases du fichier .zshrc

```bash
source ~/.zshrc
```
