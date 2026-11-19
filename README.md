# 🎧 AFTERHOURS — DJ Life Stories

> **200 € sur le compte, deux platines dans la chambre et une mère qui hurle de baisser ce fichu boucan. Objectif : devenir une légende de la nuit.**

Jeu d'arcade narratif inspiré de l'univers **Deejay Pat B** et de l'esthétique urbaine nocturne des grands classiques du jeu vidéo (*Wanted Stars*, bannières `MISSION PASSED!`, `WASTED`, `BUSTED!`, radar HUD et ambiance Jumpstyle / Old School 150 BPM).

Le fichier principal du jeu dans le dépôt est **`AFTERHOURS_DEEJAY_PAT_B_Edition.html`**.
https://github.com/asblPixels/Afterhours/blob/eb6e3b00a6696e79cc851eb4b6f0fdc823d0d6bb/AFTERHOURS_DEEJAY_PAT_B_Edition.html

## ✨ Nouveautés & Fonctionnalités

* **Identité visuelle fidèle à l'artiste :** Palette néon **Jaune Smiley (`#FFE600`)**, **Rose Néon (`#E6007E`)** et **Bleu Glace (`#7DD3E2`)**, avec le smiley iconique aux yeux en croix et langue tirée animé en temps réel.

* **Lecteur MP3 de l'artiste intégré (WebAudio Analyser) :** Charge n'importe quel fichier audio local (`.mp3`, `.wav`, `.ogg`) depuis ton téléphone ou ton ordinateur. Les caissons de basses, l'égaliseur 16 bandes et le smiley réagissent directement aux basses fréquences du morceau (avec repli automatique sur un synthé Jumpstyle 150 BPM intégré si aucun fichier n'est chargé).

* **6 Missions scénarisées :**

  1. **La Tournée des 3 Soirées :** Course poursuite nocturne sur autoroute côtière sous 5 étoiles de recherche.

  2. **Le Mec Bourré (Set Express) :** Set rythmique de 25 secondes au rythme assoupli avec gestion d'un client insistant et shout-outs de foule (`COME ON!`, `JUMP! JUMP!`, `HANDS UP!`).

  3. **L'Addition du Backstage :** Runner urbain dans une ruelle néon pour rejoindre la camionnette avant le videur.

  4. **Le Crash du Lecteur CDJ (`EMERGENCY LOOP`) :** Calage manuel du tempo (*beatmatch*) sur jogwheel pour sauver le set en plein peak-time.

  5. **L'After chez la Voisine :** Gestion du volume des caissons entre montée d'ambiance et alertes police/voisinage à la fenêtre.

  6. **Parachute sur la Mainstage :** Saut de précision avec fumigènes bicolores et gestion du vent pour atterrir derrière les platines devant 60 000 personnes.

* **Multilingue & Mobile-First :** Interface disponible en **Français (FR)**, **Anglais (EN)** et **Néerlandais (NL)**, optimisée pour écrans tactiles Android (format portrait 16:9 / `480×854`) ainsi que clavier PC.

## 🚀 Comment lancer le jeu depuis le fichier

Le jeu est entièrement contenu dans le fichier autonome **`AFTERHOURS_DEEJAY_PAT_B_Edition.html`**, sans dépendance externe ni installation requise.

### 1. En ligne (via GitHub Pages)

Si GitHub Pages est activé sur le dépôt (`Settings > Pages > Branch: main`), tu peux accéder directement au fichier depuis l'URL GitHub Pages du dépôt, par exemple :

```
https://asblpixels.github.io/Afterhours/AFTERHOURS_DEEJAY_PAT_B_Edition.html

```

### 2. Depuis le fichier téléchargé sur Android (Smartphone)

> ⚠️ **Important :** Ne lance pas le fichier depuis l'aperçu intégré de GitHub, de Google Drive ou d'une visionneuse de texte (qui affichent le code source en texte brut au lieu d'exécuter le jeu).

1. Télécharge **`AFTERHOURS_DEEJAY_PAT_B_Edition.html`** dans le dossier **Téléchargements** (`Download`) de ton téléphone.

2. Ouvre directement l'application **Google Chrome** (ou Firefox / Brave).

3. Dans la barre d'adresse, saisis le chemin local suivant :

   ```
   file:///storage/emulated/0/Download/AFTERHOURS_DEEJAY_PAT_B_Edition.html
   
   ```

4. Touche l'écran pour activer le son ou clique sur **`🎵 CHARGER SON MP3 DE L'ARTISTE`** pour importer ta musique.

### 3. Sur PC (Linux / Windows / macOS)

* **Ouverture directe :** Télécharge `AFTERHOURS_DEEJAY_PAT_B_Edition.html` puis double-clique dessus (ou **Clic droit > Ouvrir avec > Firefox / Chrome**).

* **Via un serveur local (recommandé pour le développement) :**

  ```
  git clone https://github.com/asblPixels/Afterhours.git
  cd Afterhours
  python3 -m http.server 8000
  
  ```

  Ouvre ensuite `http://localhost:8000/AFTERHOURS_DEEJAY_PAT_B_Edition.html` dans ton navigateur.

## 🎮 Contrôles

| Mission | Mobile (Tactile) | PC (Clavier) | 
| ----- | ----- | ----- | 
| **1. La Tournée** | Glisser le doigt gauche / droite | Flèches `←` / `→` | 
| **2. Le Mec Bourré** | Taper sur les 4 colonnes | Touches `A` `Z` `E` `R` | 
| **3. L'Addition** | Taper droite = Sauter · Taper gauche = Glisser | `↑` / `Espace` (Sauter) · `↓` (Glisser) | 
| **4. Crash CDJ** | Taper quand le curseur est dans la zone jaune | `Espace` ou `Entrée` | 
| **5. L'After** | Maintenir appuyé pour les basses · Relâcher à l'alerte | Maintenir `Espace` ou `↑` | 
| **6. Parachute** | Glisser le doigt gauche / droite | Flèches `←` / `→` | 

## 🛠️ Stack Technique

* **HTML5 Canvas 2D** & **CSS3** (mise à l'échelle dynamique `devicePixelRatio` 16:9).

* **WebAudio API** (synthétiseur 150 BPM procédural + lecteur `MediaElementAudioSourceNode` et `AnalyserNode` FFT).

* **Zero-dependency :** 100 % Vanilla JavaScript, polices embarquées en Base64, fonctionne hors ligne.

## 📜 Crédits & Licence

* **Création & Développement :** [Pixel's ASBL](https://asblpixels.be) — Boussu, Belgique.

* **Inspiration :** Univers musical et visuel de **Deejay Pat B** *(jeu de fan non officiel, sans affiliation commerciale avec l'artiste)*.
