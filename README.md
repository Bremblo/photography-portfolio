# Conor Schall — Photography Portfolio

Minimal photography portfolio. Leica-clean structure, Y2K neon-on-black palette.

## Adding Photos

1. Drop image files into the `photos/` folder
2. Push to GitHub
3. Done — a GitHub Action auto-generates the photo list and Netlify deploys

You never need to edit `index.html` to add or remove photos.

## Image Tips

- Resize to **1600px** on the long edge
- Save as `.jpg` at **80% quality**

## Deploy on Netlify

1. Push this repo to GitHub
2. Go to [netlify.com](https://www.netlify.com), sign in with GitHub
3. Click **New site from Git** → pick this repo
4. Leave build settings blank (no build command, publish directory: `/`)
5. Click **Deploy Site**

## How It Works

A GitHub Action (`.github/workflows/build-photo-list.yml`) watches the `photos/` folder. Whenever you push new images, it generates a `photos.txt` file listing every image. The site reads `photos.txt` on load and builds the gallery automatically.

## One-Time Setup: Contact Info

Update the contact links in `index.html` (marked with a comment near the contact section):
- Email address
- Instagram handle + URL
- YouTube URL
- Bio text on the About page
