# Ajout de paquet : ratbagd

[↩️ Retour](./README.md)

## Description

Permet de changer les paramètres des matériels gaming. Il supporte Etekcity, G.Skill, Roccat, SteelSeries et Logitech.

## 1. Installation

```bash
apt install ratbagd
```

## 2. Trouver le nom du clavier

```bash
ratbagctl list

# sortie
singing-gundi:       Logitech G915 TKL LIGHTSPEED Wireless RGB Mechanical Gaming Keyboard
```

## 3. Mettre le profil 0 actif

```bash
ratbagctl "[NOM_DU_CLAVIER]" profile active set 0
```

## 4. Mettre la lumière du G en mode continu

```bash
ratbagctl "[NOM_DU_CLAVIER]" led 0 set mode on
```

## 5. Mettre la lumière des touches en mode continu

```bash
ratbagctl "[NOM_DU_CLAVIER]" led 1 set mode on
```

## 6. Changer la couleur de la lumière du G

```bash
ratbagctl "[NOM_DU_CLAVIER]" led 0 set color [HEXADECIMAL]
```

## 7. Changer la couleur de la lumière des touches

```bash
ratbagctl "[NOM_DU_CLAVIER]" led 1 set color [HEXADECIMAL]
```
