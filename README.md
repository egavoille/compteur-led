# Compteur LED · DMX

Appli web mobile pour préparer le patch de bandeaux LED : nombre de LEDs, canaux, univers DMX et prix, avec un aperçu lumineux à l'échelle.

Version **0.8**.

## Fonctions

- Bandeaux saisis **en LEDs ou en mètres**, les deux champs étant liés par la densité (30, 60, 96, 120, 144 LEDs/m ou valeur libre).
- Types de LED : Mono (1 c), RGB (3 c), RGBW (4 c), RGB 16 bits (6 c).
- Univers et canal de départ, bandeaux **chaînés** ou **déliés** avec univers et canal propres.
- LED coupée entre deux univers **autorisée** (512 canaux remplis) ou **interdite** (170 LEDs RGB / 128 RGBW par univers), plafond de LEDs par univers optionnel.
- Détection des **conflits d'adresses**.
- **Prix** au mètre ou à la bobine : coût par bandeau, total, bobines à acheter et chute.
- **Récapitulatif** général et patch copiable en texte.
- **Aperçu lumineux** animé : couleur par univers, arc-en-ciel, chenillard, blanc, couleur libre.
- Trois habillages au choix : **Pupitre**, **Flight case**, **Plan de feux** (tirage bleu en mode sombre).

## Installation

Déposer le contenu du dépôt dans un dossier d'un site en HTTPS. `index.html` est la page de lancement.

Sur iPhone : ouvrir la page dans Safari, **Partager → Sur l'écran d'accueil**. L'appli s'ouvre en plein écran et fonctionne ensuite **hors ligne** (`sw.js`). Les réglages restent enregistrés sur l'appareil.

Pour publier une nouvelle version, changer aussi le nom du cache en tête de `sw.js`.

## Contenu

| Fichier | Rôle |
|---|---|
| `index.html` | Appli complète (v0.8) avec choix de l'habillage |
| `manifest.webmanifest`, `icons/` | Installation sur l'écran d'accueil |
| `sw.js` | Fonctionnement hors ligne |
| `versions/` | v0.7 d'origine et les trois habillages séparés |

Aucune dépendance : HTML, CSS et JavaScript écrits à la main. Seules les polices viennent de Google Fonts.
