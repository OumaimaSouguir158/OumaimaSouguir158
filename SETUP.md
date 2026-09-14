# GitHub Profile README — Setup Instructions

## Structure du repo

```
oumaima-souguir/          ← repo spécial (même nom que ton username GitHub)
├── README.md             ← le profil affiché sur github.com/oumaima-souguir
├── assets/
│   └── banner.svg        ← bannière animée (cursor clignotant)
└── .github/
    └── workflows/
        └── snake.yml     ← génère l'animation snake automatiquement
```

---

## Étape 1 — Créer le repo spécial GitHub

1. Va sur [github.com/new](https://github.com/new)
2. **Repository name :** `oumaima-souguir` *(exactement ton username)*
3. Coche **Public**
4. Coche **Add a README file**
5. Clique **Create repository**

> GitHub reconnaît automatiquement ce repo spécial et affiche son README sur ton profil.

---

## Étape 2 — Uploader les fichiers

```bash
# Clone le repo spécial que tu viens de créer
git clone https://github.com/oumaima-souguir/oumaima-souguir.git
cd oumaima-souguir

# Copie les fichiers de ce projet dedans
cp README.md ./README.md
mkdir -p assets
cp assets/banner.svg ./assets/banner.svg
mkdir -p .github/workflows
cp .github/workflows/snake.yml ./.github/workflows/snake.yml

# Commit et push
git add .
git commit -m "feat: add profile README with animations"
git push origin main
```

---

## Étape 3 — Activer l'animation Snake

1. Dans ton repo `oumaima-souguir`, va dans **Settings → Actions → General**
2. Sous "Workflow permissions", sélectionne **Read and write permissions**
3. Sauvegarde

Puis va dans **Actions → Generate Snake Animation → Run workflow**

L'animation sera générée dans la branche `output` et s'affichera automatiquement dans le README.

---

## Étape 4 — Mettre à jour les liens

Avant de pousser, remplace dans `README.md` :

| Placeholder | Ta vraie valeur |
|-------------|-----------------|
| `oumaima-souguir` (GitHub username) | ton vrai username GitHub |
| `oumaima-souguir.vercel.app` | ton URL Vercel après déploiement |
| `souguir.oumaima@hotmail.com` | ✅ déjà correct |

---

## Étape 5 — GitHub Stats (optionnel)

Les cartes `github-readme-stats` affichent tes vraies stats automatiquement
à condition que ton username GitHub soit **oumaima-souguir**.

Si différent, remplace dans le README :
```
username=oumaima-souguir  →  username=TON_VRAI_USERNAME
```

---

## Services utilisés (tous gratuits)

| Service | Rôle | URL |
|---------|------|-----|
| `readme-typing-svg` | Animation de texte dactylographié | demolab.com |
| `github-readme-stats` | Cartes stats GitHub | vercel app |
| `github-readme-activity-graph` | Graphique de contributions | vercel app |
| `Platane/snk` | Animation snake sur la grille | GitHub Actions |
| Shields.io | Badges technos | shields.io |

Tous fonctionnent sans compte supplémentaire — juste l'URL dans le Markdown.

---

## Résultat attendu

Ton profil affichera :
- ✅ Banner SVG avec curseur clignotant
- ✅ Texte dactylographié animé (rôle, stack, objectif)
- ✅ Badges LinkedIn / Email / Portfolio
- ✅ Bloc code Python `whoami`
- ✅ Tableau des 4 projets avec badges technos
- ✅ Tableau des skills par domaine
- ✅ Log style `git log` pour l'expérience
- ✅ Cartes stats GitHub live
- ✅ Graphique d'activité
- ✅ Animation snake sur la grille de contributions
- ✅ Tableau des langues parlées
