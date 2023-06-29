# Ajout de paquet : snapd

[↩️ Retour](./README.md)

## Description

Permet l'installation de nouvelles versions de logiciels.

## 1. Installation

```bash
apt install snapd
```

## 2. Activation du service snap au lancement du système

```bash
systemctl enable snapd.apparmor
```

## 3. Activation du service snap sur la session courante

```bash
service snapd.apparmor start
service snapd start
apparmor_parser -r /etc/apparmor.d/*snap-confine*
apparmor_parser -r /var/lib/snapd/apparmor/profiles/snap-confine*
```
