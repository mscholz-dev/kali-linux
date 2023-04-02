# Paquet : NVM (Node Version Manager)

## Description

Permet de changer la version de node js

## 1. Installation

```bash
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

## 2. Mettre à jour la configuration du terminal

```bash
source ~/.zshrc
```

## 3. Vérification

```bash
nvm -v
```

## 4. Installation de versions de node js

```bash
nvm install vXX.XX.XX
```

## 5. Utilisation d'une version de node js

```bash
nvm use vXX.XX.XX
```