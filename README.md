# Kleibooth

A browser-based event photobooth with custom Instax paper designs, downloadable layout guides, stickers, filters, and on-device person cutout for scene replacement.

## Run locally

Serve this folder from a local web server so the camera and asset paths work correctly:

```bash
python -m http.server 4173
```

Then open `http://localhost:4173`.

## Deploy to Vercel

Upload this folder to a Git repository, import it in Vercel, and use the default static-site settings. No build command or output directory is required.

Camera access requires HTTPS in production, which Vercel provides. Kleibooth includes its MediaPipe runtime and person-segmentation model locally, so background replacement does not depend on third-party downloads.
