# Ajout de paquet : foremost

[↩️ Retour](./README.md)

## 1. Installation

```bash
apt install foremost
```

## 2. Lister les disques disponibles

```bash
fdisk -l
```

## 3. Récupération des fichiers d'un disque

```bash
foremost -t all -i /dev/[NOM_DU_DISQUE] -v -o /[CHEMIN_DE_SORTIE]
```
