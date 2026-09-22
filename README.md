# Kleibooth

A browser-based event photobooth with custom Instax paper designs, downloadable layout guides, draggable stickers, live camera face props for up to two faces, eight photo filters, and on-device person cutout for scene replacement.

Version 4.3 adds transparent anime-blush and moustache props that follow each face and are baked into the finished photos. The refreshed filter set includes Natural, Warm, B&W, Cool, Soft, Film, Vivid, and Dreamy looks.

## Run locally

Serve this folder from a local web server so the camera and asset paths work correctly:

```bash
python -m http.server 4173
```

Then open `http://localhost:4173`.

## Deploy to Vercel

Upload this folder to a Git repository, import it in Vercel, and use the default static-site settings. No build command or output directory is required.

Camera access requires HTTPS in production, which Vercel provides. Kleibooth includes its MediaPipe runtime, face-landmark model, and person-segmentation model locally, so its visual effects do not depend on third-party AI downloads.
