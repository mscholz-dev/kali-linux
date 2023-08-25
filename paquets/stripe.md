# Ajout de paquet : stripe CLI

[↩️ Retour](./README.md)

## Description

Permettre l'écoute et le teste de son intégration stripe

## 1. Ajoutez la clé GPG de la CLI Stripe au trousseau de clés des sources apt

```bash
curl -s https://packages.stripe.dev/api/security/keypair/stripe-cli-gpg/public | gpg --dearmor | sudo tee /usr/share/keyrings/stripe.gpg
```

## 2. Ajoutez le référentiel apt de la CLI à la liste des sources apt

```bash
echo "deb [signed-by=/usr/share/keyrings/stripe.gpg] https://packages.stripe.dev/stripe-cli-debian-local stable main" | sudo tee -a /etc/apt/sources.list.d/stripe.list
```

## 3. Mettez à jour la liste des paquets

```bash
sudo apt update
```

## 4. Installez la CLI

```
sudo apt install stripe
```

## 5. S'identifier

```
stripe login
```
