# Ajout de paquet : xrdp

[↩️ Retour](./README.md)

## 1. Installation

```bash
apt install xrdp
```

## 2. Activaction du lancement automatique

```bash
update-rc.d xrdp enable
```

## 3. Démarrer le service xrdp

```bash
service xrdp start
```

## 4. Vérifier que le service xrdp est activé

```bash
service xrdp status
```

## 5. Créer un nouvel utilisateur pour s'y connecter à distance

```bash
adduser --home /home/[NOM] [NOM]
# Full Name []: [USER]
```

## 6. Ajojuter le privilège sudo au nouvel utilisateur

```bash
usermod -aG sudo [NOM]
```
