# UnReel Website (GitHub Pages Ready)

This repository contains a responsive, semantic, static site for **UnReel** designed to deploy on GitHub Pages.

## Project Structure

```text
/
├── index.html
├── styles.css
├── README.md
└── assets/
    ├── needfinding.pdf
    ├── gr2_slides.pdf
    └── video.mp4
```

## Deploy to GitHub Pages

1. Create a GitHub repository (or use your existing one).
2. Push this project to the default branch (`main` is recommended).
3. In your GitHub repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**.
6. Wait for deployment to finish. Your site will be available at:
   - `https://<username>.github.io/<repository-name>/` (project site), or
   - `https://<username>.github.io/` (user/org site if repo is named `<username>.github.io`).

## Push to GitHub (Command Line)

Run these commands from the repository root:

```bash
git init
git add .
git commit -m "Initial UnReel website"
git branch -M main
git remote add origin https://github.com/<username>/<repository-name>.git
git push -u origin main
```

If your repo already exists locally with a remote configured:

```bash
git add .
git commit -m "Update website content"
git push
```

## Where to Upload Deliverable PDFs

Place all PDFs and downloadable assets in the `assets/` directory.

Current required files used by the site:

- `assets/needfinding.pdf`
- `assets/gr2_slides.pdf`
- `assets/video.mp4`

Additional planned deliverables can be added to `assets/` and linked from `index.html` using relative paths, for example:

- `./assets/final-report.pdf`
- `./assets/poster.pdf`
- `./assets/demo-video.mp4`

## Notes

- The site uses only relative internal paths for project files.
- Layout and typography are optimized for desktop and mobile.
- You can replace placeholder assets in `assets/` without changing site structure.
