# WASSCE Study — GitHub Pages deployment

## Why a blank page can appear
This project is a Vite + React + TypeScript application. GitHub Pages cannot execute the `.tsx` source directly. The site must first be built into `dist/`.

This project now includes `.github/workflows/deploy-pages.yml`, which builds the app automatically whenever `main` is updated.

## Deploy
1. Upload/commit the contents of this project to the GitHub repository `Wassce-past-questions-`.
2. Push to the `main` branch.
3. In GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Wait for the **Deploy WASSCE Study to GitHub Pages** workflow to finish.
5. Open:
   `https://abdulsammedtakiyudeen-bot.github.io/Wassce-past-questions-/`

The Vite base path is already configured for that repository.

## Important
Do not open the repository's raw `src/main.tsx` as the website. The deployed site is the generated `dist/` output produced by the workflow.
