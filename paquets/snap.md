# Ajout de paquet : snap

[↩️ Retour](./README.md)

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
```
