# Penché

Générateur de titres déformés en perspective, exportables en SVG vectoriel.

- Inclinaison **horizontale** (grandit à droite ou à gauche, lentille, sablier) et **verticale**
- Intensité, ancrage (haut, centre, bas), interlettrage réglables
- 2 couleurs libres (texte et fond)
- 86 polices Google Fonts intégrées, ou **ajoutez la vôtre** (.ttf, .otf, .woff) par glisser-déposer
- Export SVG : de vrais tracés, sans police à embarquer

## Utiliser

Ouvrez `index.html` dans un navigateur. Tout tourne en local, sans serveur ni compte.
Le seul chargement externe est [opentype.js](https://opentype.js.org) (MIT) depuis cdnjs.

Pour l'héberger : GitHub Pages (Settings → Pages → branche `main`, dossier racine).

## Comment ça marche

Chaque lettre est convertie en contours (opentype.js), normalisée sur la hauteur de capitale,
puis chaque point est déplacé selon deux profils : la hauteur varie avec la position horizontale,
la largeur varie avec la position verticale. Le résultat est un unique `<path>` SVG.

## Licences

- Code : MIT, voir `LICENSE`.
- Polices intégrées : issues de Google Fonts via Fontsource, sous licences libres
  (SIL Open Font License 1.1 pour la grande majorité, certaines sous Apache 2.0).
  Chaque police reste la propriété de ses auteurs. Les SVG exportés sont utilisables
  librement, selon la licence de la police choisie.

Créé par [Jordan Boutin](https://jordanboutin.fr).
