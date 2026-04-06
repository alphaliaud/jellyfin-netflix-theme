# 🎬 Jellyfin Netflix Theme

Un thème CSS pour [Jellyfin](https://jellyfin.org) inspiré de l'interface Netflix.

---

## 📸 Aperçu

| Couleur principale | Accent | Font display | Font corps |
|--------------------|--------|--------------|------------|
| `#141414`          | `#E50914` (rouge Netflix) | Bebas Neue | Barlow |

---

## 🚀 Installation via CDN

### Option A — jsDelivr (recommandé)

Une fois le dépôt public sur GitHub, ton CSS est automatiquement
disponible via jsDelivr **sans configuration** :

```
https://cdn.jsdelivr.net/gh/alphaliaud/jellyfin-netflix-theme@main/theme.css
```

**Dans Jellyfin :**
1. Tableau de bord → Général → CSS personnalisé
2. Coller :

```css
@import url('https://cdn.jsdelivr.net/gh/alphaliaud/jellyfin-netflix-theme@main/theme.css');
```

3. Enregistrer → Rafraîchir le navigateur.

### Option B — URL brute GitHub (pas de cache CDN)

```
https://raw.githubusercontent.com/alphaliaud/jellyfin-netflix-theme/main/theme.css
```

> ⚠️ GitHub bloque parfois les raw URLs dans les CSS `@import`.
> Préfère jsDelivr.

### Option C — Versioning (pour épingler une version stable)

Crée un **tag Git** pour figer une version :

```bash
git tag v1.0.0
git push origin v1.0.0
```

Puis utilise :
```
https://cdn.jsdelivr.net/gh/alphaliaud/jellyfin-netflix-theme@v1.0.0/theme.css
```

---

## 🛠️ Créer le dépôt GitHub (étape par étape)

```bash
# 1. Initialiser le repo local
git init
git add theme.css README.md
git commit -m "feat: initial Netflix theme"

# 2. Créer le repo sur GitHub (nécessite gh CLI ou interface web)
gh repo create jellyfin-netflix-theme --public --source=. --push
# ou depuis https://github.com/new → uploader les fichiers

# 3. Le CDN jsDelivr est actif immédiatement après le push !
```

---

## ✏️ Personnalisation

Toutes les variables sont dans `:root` en haut du CSS :

```css
:root {
  --netflix-red:   #E50914;   /* Changer la couleur d'accent */
  --bg-primary:    #141414;   /* Fond principal */
  --font-body:     'Barlow';  /* Police du texte */
  --font-display:  'Bebas Neue'; /* Police des grands titres */
}
```

---

## 📁 Structure du dépôt

```
jellyfin-netflix-theme/
├── theme.css      ← fichier principal
└── README.md
```

---

## 📝 Licence

MIT — Libre de modifier et redistribuer.
