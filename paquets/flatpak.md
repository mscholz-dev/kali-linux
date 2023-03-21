# Ajout de paquet : flatpak

[↩️ Retour](./README.md)

## 1. Installation de flatpak

```bash
apt install flatpak
```

## 2. Installation du plugin logiciel flatpak pour debian

```bash
apt install gnome-software-plugin-flatpak
```

## 3. Ajouter le dépôt flathub

```bash
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

## 4. Redémarrer le système

```bash
reboot
```
