# Déploiement sur Vercel — Guide complet

## Prérequis
- Un compte GitHub (gratuit)
- Un compte Vercel (gratuit) → vercel.com

---

## Étape 1 — Mettre le projet sur GitHub

```bash
# Dans le dossier web_version/
git init
git add .
git commit -m "Acoustique 3D — PEN"

# Sur GitHub : créer un nouveau repo "acoustique-3d-pen"
git remote add origin https://github.com/TON_USERNAME/acoustique-3d-pen.git
git push -u origin main
```

## Étape 2 — Connecter à Vercel

1. Va sur https://vercel.com
2. Clique "Add New Project"
3. Connecte ton GitHub → sélectionne "acoustique-3d-pen"
4. Vercel détecte automatiquement que c'est un site statique
5. Clique "Deploy" → c'est tout !

## Étape 3 — Ton lien

Vercel te donne un lien du type :
```
https://acoustique-3d-pen.vercel.app
```

Ce lien est public, tu peux le partager au jury directement !

## Mise à jour

À chaque `git push`, Vercel redéploie automatiquement.

```bash
git add .
git commit -m "Mise à jour"
git push
# → Vercel redéploie en ~30 secondes
```

## Structure à mettre sur GitHub

```
(racine du repo)
├── public/
│   └── index.html    ← L'app Three.js complète
├── package.json
├── vercel.json
└── DEPLOY.md
```
