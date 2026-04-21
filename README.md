# nautika-website

Source for www.nautikacorp.com, hosted on Firebase Hosting (project: `nautikacorpcom`).

## Layout

- `index.html`, `apps.html` — edited at the repo root (tracked in git).
- `public/` — what Firebase actually deploys. Copy edited HTML files here before deploying.
- `public/css/style.css` — shared styles.
- `firebase.json`, `.firebaserc` — Firebase Hosting config.

## Deploy

1. Edit the HTML files at the repo root.
2. Copy them into `public/`:
   ```
   cp index.html apps.html public/
   ```
3. Make sure you're logged in as an account with Owner access to the `nautikacorpcom` Firebase project:
   ```
   firebase login:list
   ```
   If not, run `firebase login` (or `firebase login --reauth`) and sign in.
4. Deploy:
   ```
   firebase deploy
   ```

## Access

Owner access is managed in the GCP IAM console for the `nautikacorpcom` project. Workspace super admins for `nautikacorp.com` can grant themselves Owner via the Organization IAM page if needed.
