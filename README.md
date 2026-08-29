# GUDithering

**GUDithering by [ohmygud.com](https://ohmygud.com)** is a client-side image editor for limited-palette dithering, distressed print effects and palette-based image processing.

## Features

- Floyd–Steinberg, Atkinson, Bayer 4×4, Bayer 8×8 and Threshold dithering
- Thematic palette groups plus editable custom colors, including a dedicated **Gothic Girlcore** set (Cherry Bow, Strawberry Milk, Butter Baby, Angel Cake, Hot Ribbon, Powder Room)
- Image controls: brightness, contrast, saturation, grain, paper fade, scanlines, distress
- Presets and random parameter mutation
- HD PNG export from the original source image
- HD PDF export at 150 / 300 / 600 DPI
- Responsive mobile UI with a pink / butter-yellow Gothic Girlcore interface skin
- No backend and no image upload: processing happens locally in the browser
- Export/import-friendly settings JSON

## Run locally

Open `index.html` directly, or serve the folder with any static server.

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## GitHub Pages

1. Create a repository and put `index.html` in its root.
2. Push to GitHub.
3. In **Settings → Pages**, choose **Deploy from a branch**.
4. Select `main` and `/ (root)`.

The site is entirely static. The only external runtime dependency is jsPDF, loaded from jsDelivr for PDF export.

## Notes

Very large exports are capped automatically to avoid browser memory crashes. The editor keeps the preview lightweight, while export rendering starts again from the original image.

## Branding

GUDithering by ohmygud.com
