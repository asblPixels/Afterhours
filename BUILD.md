# Reconstruire l'APK

L'APK est une simple application Android qui affiche `index.html` en plein écran dans une WebView,
en mode portrait. Elle ne demande aucune permission.

## Ce qu'il faut

- Java 17 ou plus récent
- [Apktool](https://github.com/iBotPeaches/Apktool/releases) (testé avec la version 2.12.0)
- [uber-apk-signer](https://github.com/patrickfav/uber-apk-signer/releases) (testé avec la 1.3.0)

## Étapes

```bash
# 1. copier la version à jour du jeu dans les assets
mkdir -p assets && cp ../index.html assets/index.html

# 2. construire
java -jar apktool.jar b . -o unsigned.apk

# 3. aligner et signer
java -jar uber-apk-signer.jar --apks unsigned.apk -o out

# 4. vérifier
java -jar uber-apk-signer.jar -y --apks out/*.apk
```

## Signature

L'APK publié est signé avec la **clé de débogage par défaut d'uber-apk-signer**, identique pour
tout le monde : n'importe qui peut donc reconstruire une mise à jour qui s'installe par-dessus la
version publiée. Pour une vraie distribution, remplacer cette clé par une clé privée gardée hors
du dépôt (`--ks ma-cle.jks`), et ne jamais la committer.

## Contenu

- `AndroidManifest.xml` — package `be.asblpixels.afterhours`, portrait, plein écran, Android 7+
- `smali/be/asblpixels/afterhours/MainActivity.smali` — l'activité WebView
- `res/mipmap-*/ic_launcher.png` — l'icône
- `apktool.yml` — version et cibles SDK
