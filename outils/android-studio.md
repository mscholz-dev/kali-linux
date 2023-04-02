# Outils : Android studio

## Description

Permet d'émuler un appareil android mobile.

## 1. Installer l'exécutable

Se rendre sur ce lien : https://developer.android.com/studio/install?hl=fr

## 2. Extraire l'exécutable

```bash
tar -xvzf android-studio-2022.1.1.21-linux.tar.gz
```

## 3. Ajouter des dépendances

```bash
apt install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386
```

## 4. Ajouter android studio au répertoire /usr/local

```bash
mv ~/Téléchargement/android-studio /usr/local
```

## 5.Exécuter android studio

```bash
cd /usr/local/android-studio/bin
./studio.sh
```

## 6. Installer et activer KVM

```bash
apt install cpu-checker qemu-kvm libvirt-bin ubuntu-vm-builder bridge-utils ia32-libs-multiarch
egrep -c "(vmx|svm)" /proc/cpuinfo
kvm-ok
```

## 7. Ajouter les variables d'environnements ANDROID_HOME

```bash
nano .zshrc
```

Ajouter à la fin du fichier les variables d'environnements d'android studio

```bash
# android studio
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

## 9. Accepter des licences dans android studio

Dans android studio, aller dans "SDK manager" > "SDK Tools" et cocher la première checkbox "Android SDK Build-Tools 31-rc5".
