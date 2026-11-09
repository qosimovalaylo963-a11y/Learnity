# Learnity — Lively Teaching & Mentorship Project

This repository contains the Learnity website as a static HTML page.

## Run locally

Open `index.html` in a modern browser. The page loads Tailwind CSS, Google Fonts, Lucide icons, and some photos from external CDNs, so an internet connection is needed for those assets.

## Publish with GitHub Pages

1. Create a new GitHub repository (for example, `learnity`).
2. Upload `index.html`, `.nojekyll`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch **main** and folder **/(root)**, then click **Save**.
6. After deployment completes, use the URL shown in the Pages section.

## Important: backend functionality

GitHub Pages hosts static files only. This HTML page includes frontend calls to `/api/...` for authentication, applications, dashboards, and saved site content. Those API routes need a separately deployed backend and database. Without that backend, the public page may load, but these features will not work as a shared production system.

The HTML also contains demo seed accounts and demo passwords in client-side JavaScript. Anyone who can view the source can read them. Do not put real passwords, private user data, API secrets, or production credentials in this file or in a public repository. Replace the demo authentication with a secure server-side implementation before using real accounts.
