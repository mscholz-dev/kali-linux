## Trouver la valeur "windowid" de la fenêtre à enregistrer

```bash
xwininfo -display :0
```

## Enregistrer tous les écrans (30 FPS)

```bash
recordmydesktop --fps=30 --s_quality=10
```

## Enregistrer une fenêtre spécifique (30 FPS)

```bash
# remplacer la valeur "0x4200006" par celle de votre fenêtre
recordmydesktop --fps=30 --s_quality=10  --windowid=0x4200006
```

## Enregister le second écran uniquement

```bash
recordmydesktop --fps=30 --s_quality=10 --x=1920
```
