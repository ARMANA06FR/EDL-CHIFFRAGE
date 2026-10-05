# EDL 06 IMMO

Application web d’état des lieux (PWA) : comparatif entrée/sortie, chiffrage, catalogue.

## Utilisation rapide

1. Publie ce dossier sur **GitHub Pages** (voir ci-dessous)
2. Ouvre l’URL sur ton téléphone
3. **Ajouter à l’écran d’accueil** (Safari iOS / Chrome Android)

Fonctionne hors ligne après la première visite (service worker).

## Mettre en ligne sur GitHub (3 minutes)

### A. Créer le dépôt

1. Va sur [github.com/new](https://github.com/new)
2. Nom du dépôt : par ex. `edl` (public)
3. **Ne coche pas** “Add a README” si tu envoies déjà ces fichiers
4. Crée le dépôt

### B. Envoyer les fichiers

Sur ton ordinateur, dans ce dossier :

```bash
git init
git add .
git commit -m "EDL 06 IMMO PWA"
git branch -M main
git remote add origin https://github.com/TON_COMPTE/edl.git
git push -u origin main
```

(Remplace `TON_COMPTE` et `edl` par ton nom GitHub et le nom du dépôt.)

Tu peux aussi glisser-déposer les fichiers sur github.com (onglet **uploading an existing file**).

### C. Activer GitHub Pages

1. Dépôt → **Settings** → **Pages**
2. Source : **Deploy from a branch**
3. Branch : **main** / dossier **/ (root)**
4. **Save**

Après 1–2 minutes, l’app est en ligne :

```
https://TON_COMPTE.github.io/edl/
```

### D. Installer sur le téléphone

- **Android (Chrome)** : menu ⋮ → **Installer l’application** ou **Ajouter à l’écran d’accueil**
- **iPhone (Safari)** : bouton Partager → **Sur l’écran d’accueil**

## Fichiers

| Fichier | Rôle |
|---------|------|
| `index.html` | Application |
| `manifest.json` | Nom, icônes, mode plein écran |
| `service-worker.js` | Cache offline |
| `icon-192.png` / `icon-512.png` | Icônes |

## Données

Tout reste **dans le navigateur** du téléphone (`localStorage`).  
Pense à **Exporter JSON** régulièrement pour sauvegarder.
