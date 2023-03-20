# Ajout de paquet : snap

## 1. Installation

```bash
sudo apt install snapd
```

## 2. Activation du service snap au lancement du système

```bash
sudo systemctl enable snapd.apparmor
```

## 3. Activation du service snap sur la session courante

```bash
sudo service snapd.apparmor start
```
