# Fonctionnalité : bluetooth

## Description

Permet d'activer le bluetooth et d'avoir une interface graphique fonctionnelle pour rechercher et se connecter à des appareils.

## 1. Installation

```bash
apt install bluetooth bluez bluez-tools rfkill
```

## 2. Activer la connexion sans fil

```bash
rfkill unblock bluetooth
```

## 3. Activation du bluetooth

```bash
service bluetooth start
```

## 4. Ajout du gestionnaire de connexion bluetooth

```bash
apt install blueman
```
