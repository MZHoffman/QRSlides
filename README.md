# QRSlides

A small, local-only QR slideshow. Each slide displays a QR image next to a title and description. Slides advance every 15 seconds; the bottom bar counts down. Left and right arrow keys change slides immediately. Click anywhere on the presentation to open the hidden slide editor.

Slide metadata is saved in `slides.json`, and uploaded images are saved in `pictures/`. This repository includes the current slides and their pictures. No Firebase account or hosted service is needed.

## Run locally

Requires Node.js 22.13 or newer.

```bash
npm install
npm run dev
```

Open <http://127.0.0.1:4327/>. The local data server uses port 4328. Both ports are fixed so a port conflict produces an error instead of silently opening the wrong app.

For a production build, run `npm run build`, then `npm run start`. The app still needs its local data server; it is not a static-only site.

## Share carefully

The pictures and slide text in this public repository are visible to everyone. Future edits made in the app remain on your machine until you commit and push the updated `slides.json` and `pictures/` files.
