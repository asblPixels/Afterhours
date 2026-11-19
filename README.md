# AFTERHOURS — DJ Life Stories

Un mini-jeu de carrière de DJ en 4 missions, jouable au doigt sur téléphone et au clavier sur PC.
Un seul fichier HTML, aucune dépendance, aucune connexion requise.

**D'après une idée originale de DJ Pat B**, publiée sur sa page Facebook officielle.
**Projet de fan non officiel, sans aucun lien avec l'artiste** — voir [DROITS.md](DROITS.md).

Réalisé par [Pixel's ASBL](https://facebook.com/asblpixels) (Boussu, Belgique).

---

## Jouer

- **Navigateur** : ouvrir `index.html` — ou la page GitHub Pages du dépôt si elle est activée.
- **Android** : installer [`release/Afterhours-DJ-Life-Stories-v1.2.apk`](release/) (92 Ko, Android 7+).
  L'application ne demande **aucune permission**, pas même l'accès à Internet.

Langues disponibles : **français, anglais, néerlandais** (boutons FR / EN / NL sur l'écran titre).

## Les 4 missions

| # | Mission | Ce qu'il faut faire |
|---|---------|---------------------|
| 1 | La tournée des 3 soirées | Rejoindre le lieu B avant la fin du chrono, set avancé de 30 min et police aux trousses |
| 2 | Le mec bourré | Tenir le dancefloor au rythme, et gérer le gars qui redemande le même morceau pour la 6e fois |
| 3 | L'addition du backstage | Fuir sur 100 m avec le sac de vinyles, sauter et glisser pour semer la sécurité |
| 4 | Parachute sur la mainstage | Sauter du jet privé et atterrir pile sur la scène malgré le vent |

Chaque mission rapporte ou coûte du **Respect** et du **cash**. Le total détermine le rang final,
de « DJ de mariage à Boussu » à « Légende de l'afterhours ».

## Technique

- `index.html` — tout le jeu : canvas 2D, interface, 3 langues, police embarquée en base64.
- Musique et bruitages **générés à l'exécution** par la Web Audio API : aucun échantillon audio,
  donc aucun contenu sonore sous droits.
- Tous les visuels sont dessinés en vectoriel dans le code. Aucune image importée.
- `android/` — les sources de l'APK (manifeste, activité WebView en smali, icônes). Voir
  [android/BUILD.md](android/BUILD.md) pour reconstruire le fichier.

## Licence

Le **code et les visuels** de ce dépôt sont publiés sous licence MIT (voir [LICENSE](LICENSE)),
© 2026 Pixel's ASBL.

L'**idée de départ** n'appartient pas à Pixel's ASBL : elle est de DJ Pat B et lui reste acquise.
La licence MIT ne porte que sur le code écrit par l'ASBL.

---

## English

A four-mission DJ career mini-game, playable with one finger on a phone or with the keyboard on a
PC. Single HTML file, no dependencies, works fully offline. Available in French, English and Dutch.

**Based on an original idea by DJ Pat B**, posted on his official Facebook page.
**Unofficial fan project, not affiliated with the artist** — see [DROITS.md](DROITS.md).

All music and sound effects are generated at runtime with the Web Audio API, and every visual is
drawn in code: the repository contains no third-party audio, images, logos or trademarks. The MIT
licence covers the code written by Pixel's ASBL only — the original idea remains DJ Pat B's.

## Nederlands

Een mini-game over een dj-carrière in 4 missies, speelbaar met één vinger op de telefoon of met het
toetsenbord op de pc. Eén HTML-bestand, geen afhankelijkheden, volledig offline. Beschikbaar in het
Frans, Engels en Nederlands.

**Naar een origineel idee van DJ Pat B**, geplaatst op zijn officiële Facebookpagina.
**Onofficieel fanproject, geen band met de artiest** — zie [DROITS.md](DROITS.md).

Alle muziek en geluidseffecten worden tijdens het spelen gegenereerd met de Web Audio API en alle
beelden zijn in code getekend: de repository bevat geen audio, afbeeldingen, logo's of merken van
derden. De MIT-licentie dekt alleen de code van Pixel's ASBL — het oorspronkelijke idee blijft van
DJ Pat B.
