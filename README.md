# Classification des végétations CBNB — PWA

Application HTML autonome de consultation de la classification physionomique et phytosociologique des végétations du CBNB.

## Contenu du dépôt

```text
/
├── index.html
├── manifest.webmanifest
├── service-worker.js
├── .nojekyll
└── icons/
    ├── favicon.svg
    ├── icon-192.png
    ├── icon-512.png
    ├── maskable-192.png
    ├── maskable-512.png
    ├── apple-touch-icon.png
    └── icon-preview.png
```

## Publication sur GitHub Pages

1. Créer un nouveau dépôt GitHub.
2. Déposer tous les fichiers présents dans ce dossier à la racine du dépôt.
3. Aller dans **Settings → Pages**.
4. Dans **Build and deployment**, choisir **Deploy from a branch**.
5. Sélectionner la branche `main` et le dossier `/root`.
6. Enregistrer, puis attendre la publication de l’URL GitHub Pages.

## Installation smartphone

### Android / Chrome

1. Ouvrir l’URL GitHub Pages de l’application.
2. Ouvrir le menu Chrome.
3. Choisir **Installer l’application** ou **Ajouter à l’écran d’accueil**.

### iPhone / Safari

1. Ouvrir l’URL GitHub Pages dans Safari.
2. Appuyer sur le bouton **Partager**.
3. Choisir **Ajouter à l’écran d’accueil**.

## Notes techniques

- L’application reste un HTML autonome enrichi en PWA.
- Le manifeste déclare les icônes, le mode `standalone`, les couleurs et l’URL de démarrage.
- Le service worker met en cache les ressources applicatives principales.
- Le fonctionnement hors ligne dépend du premier chargement complet depuis une URL HTTPS.
- Après modification de `index.html`, augmenter éventuellement la constante `CACHE_NAME` dans `service-worker.js` pour forcer la mise à jour du cache.
