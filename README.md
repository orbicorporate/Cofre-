# COFRE App

Prototype for the COFRE savings-vault gamification app. Built with React 18 + Vite + Tailwind CSS.

## Run locally

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

Output goes to `dist/`.

## Publish to GitHub + Vercel

This folder is already a git repository with one commit. To publish:

### 1. Create a GitHub repo

Go to https://github.com/new, create an empty repository (do **not** initialize it with a README), e.g. `cofre-app`. Then, from inside this folder:

```bash
git remote add origin https://github.com/SEU_USUARIO/cofre-app.git
git branch -M main
git push -u origin main
```

(Replace `SEU_USUARIO` with your GitHub username, and the repo name if you used a different one.)

### 2. Deploy on Vercel

1. Go to https://vercel.com/new
2. Click "Import" next to the `cofre-app` repository (Vercel will ask you to connect your GitHub account the first time)
3. Vercel auto-detects Vite — leave the defaults (Build Command: `vite build`, Output Directory: `dist`)
4. Click **Deploy**

That's it — every future `git push` to `main` will auto-deploy a new version.

## Project structure

```
index.html          # HTML entry point
src/main.jsx         # React entry point
src/App.jsx           # The whole app (all screens, components, design tokens)
src/index.css         # Tailwind entry + a couple of small global rules
tailwind.config.js
postcss.config.js
vite.config.js
```
