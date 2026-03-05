# Conor Schall — Photography Portfolio

Minimal photography portfolio with a web-based CMS for managing photos and content.

## Setup (one time)

1. Push this repo to GitHub
2. Go to [netlify.com](https://www.netlify.com) and sign in with GitHub
3. Click **New site from Git** → pick this repo
4. Leave build settings blank (publish directory: `/`) → click **Deploy Site**
5. In Netlify dashboard: go to **Integrations → Netlify Identity** → click **Enable Identity**
6. Under Identity settings: set **Registration** to **Invite only**
7. Click **Identity** tab → **Invite users** → enter your email
8. Go to **Integrations → Git Gateway** → click **Enable Git Gateway**
9. Check your email for the invite, set a password
10. Visit `yoursite.netlify.app/admin/` and log in

## Adding Photos

1. Go to `yoursite.netlify.app/admin/`
2. Click **Gallery → Photos**
3. Click **Add photos** to upload images
4. Click **Publish** when done

Photos are uploaded through the browser. No code, no Git, no terminal.

## Editing About / Contact

Same CMS dashboard under **Settings → About Page** or **Settings → Contact Info**.

## File Structure

```
index.html              ← the site
admin/index.html        ← CMS login page
admin/config.yml        ← CMS configuration
gallery.json            ← photo list (managed by CMS)
content/about.json      ← about page content (managed by CMS)
content/contact.json    ← contact info (managed by CMS)
photos/                 ← uploaded images (managed by CMS)
```
