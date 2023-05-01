# Outils : Mise en place d'un proxy

## Description

Permet de masquer son IP selon le proxy utilisé

## 1. Installer du paquets Tor

```bash
apt install tor
```

## 2. Modification de la configuration du proxy

```bash
nano /etc/proxychains.conf

# décommenter la ligne suivante
dynamic_chain

# commenter la ligne suivante
strict_chain

# décommenter la ligne suivante
Proxy DNS requests - no leak for DNS data

# ajouter un proxy à la fin du fichier
# liste de proxy public : www.proxynova.com/proxy-server-list/
# choisissez un proxy "Elite" afin qu'il cache votre IP lors de vos futures navigations

# exemple de proxy à ajouter
socks5 165.73.129.10 56975
```

## 3. Lancer le service Tor

```bash
service tor start
```

## 4. Utiliser le proxy

```bash
proxychains firefox [URL]
```

## 5. Vérifier que l'IP de votre proxy est différente de celle de votre router

1. Rendez-vous sur le site "whatsmyip" avec Firefox sans le proxy ;
2. Rendez-vous sur le site "whatsmyip" avec Firefix avec le proxy ;

Si les deux IP version 4 (XXX.XXX.XXX.XXX) sont différentes, alors votre proxy fonctionne !
