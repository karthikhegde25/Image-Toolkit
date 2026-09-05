# Image Toolkit

A single-file, no-build web app for everyday image editing — convert formats, compress,
watermark, filter, rotate/flip, strip metadata, and more. Everything runs **entirely in
your browser** (Canvas 2D + File APIs). No images are ever uploaded anywhere.

Built for mobile browsers but works anywhere — just open `index.html`.

## Features

| Tool | What it does |
|---|---|
| **Convert** | PNG, JPG, WEBP, BMP, ICO — single image or batch (with rotate applied per-batch), batch downloads as a ZIP |
| **Compress** | JPG/WEBP quality control, shows before/after size |
| **Increase size** | Pads a JPG/PNG with extra metadata (custom letters, up to 50 MB) |
| **Strip metadata** | Reads real EXIF tags (camera, GPS, timestamps) and PNG metadata chunks, lets you remove specific fields — or wipe everything via re-encode |
| **Watermark** | Text overlay with position, size, opacity — single or batch |
| **Filters** | Grayscale, sepia, invert, vintage, warm/cool tone, posterize, threshold, vignette, blur, sharpen, plus brightness/contrast — single or batch |
| **Rotate & flip** | 90°/180°/270° rotation and horizontal/vertical mirroring — single or batch |

Every tool that produces one image lets you type a custom output filename. Every batch
tool lets you name the resulting ZIP archive too.

## Getting started

### Run it locally
No build step, no dependencies to install. Just open `index.html` in a browser.

### Deploy with GitHub Pages
1. Create a new GitHub repository.
2. Add these files to it: `index.html`, `README.md`, `LICENSE`.
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose the `main` branch and the `/ (root)` folder, then **Save**.
5. GitHub will publish the site at:
   `https://<your-username>.github.io/<your-repo-name>/`
   (this can take a minute or two the first time)

## Uploading to GitHub

**Option A — GitHub's web UI (no command line needed)**
1. Go to [github.com/new](https://github.com/new) and create a repository.
2. On the new repo's page, click **"uploading an existing file"**.
3. Drag in `index.html`, `README.md`, and `LICENSE`.
4. Commit directly to `main`.

**Option B — git command line**
```bash
git init
git add .
git commit -m "Initial commit: Image Toolkit"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```

## File structure

```
.
├── index.html   # the entire app — HTML, CSS, and JS in one file
├── README.md
└── LICENSE
```

## How it works / privacy

- Image processing uses the browser's `<canvas>` element and the File API.
- ZIP archives (for batch downloads) are built client-side with a small hand-written,
  dependency-free ZIP writer (uncompressed "store" method).
- EXIF metadata is parsed and rewritten directly at the byte level — no libraries.
- The only network requests the page makes are for two Google Fonts (Space Grotesk,
  Inter). Everything else — every image you load, edit, and download — never leaves
  your device.

## Browser support

Any modern browser: Chrome, Firefox, Safari, Edge — desktop or mobile. Uses standard
Canvas 2D, File, Blob, and DataView APIs.

## License

MIT — see [LICENSE](./LICENSE).
