# Deploy CourseKit for free (Android / Cloudflare Pages)

## 1. Upload files to GitHub

The repository already has a README.md. Keep it. Upload these new files (including the src and public folders) to your repo `dhanaseelan-a/coursekit-mvp` on the main branch. The easiest way on Android is to unzip this archive in your phone's Files app, then use GitHub's web uploader in Chrome with **Desktop site** enabled. If the uploader fails to select nested folders, use a mobile code editor with Git support or GitHub's web editor (press `.` in desktop GitHub) to create the files one by one.

## 2. Connect Cloudflare Pages

- Sign in to https://dash.cloudflare.com/
- Workers & Pages > Create > Pages > Connect to Git
- Authorize Cloudflare access to the repository if prompted.
- Choose `dhanaseelan-a/coursekit-mvp` and the `main` branch.
- Framework preset: Vite (if offered).
- Build command: `npm run build`
- Build output directory: `dist`
- Root directory: `/` (repository root).
- No environment variables required for this frontend-only demo.
- Click Save and Deploy. Open the generated `pages.dev` URL.

## What this demo does (and does not do)

Working: responsive layout, navigation, course category filters, sample course previews, interactive JavaScript quiz.
Not yet implemented: authentication, admin, purchases, secure PDF downloads, database, backend, and Claude API integration.

## Local commands

```
npm install
npm run dev
npm run build
```

No paid infrastructure or API keys are needed to deploy the preview. The Google Fonts CSS loads from an external CDN (optional: replace with system fonts for a fully self-hosted frontend).
