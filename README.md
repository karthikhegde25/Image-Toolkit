<p align="center">
  <img src="logo.png" alt="Image Toolkit logo" width="140">
</p>

<h1 align="center">Image Toolkit</h1>

<p align="center">
  Every image tool, right on your device.<br>
  Convert, compress, crop, resize, clean and edit photos in your browser. Nothing is ever uploaded.
</p>

<p align="center">
  <a href="https://github.com/karthikhegde25/Image-Toolkit/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-0071e3"></a>
  <img alt="No build step" src="https://img.shields.io/badge/build-none-30b158">
  <img alt="Single file" src="https://img.shields.io/badge/single-file-af52de">
  <img alt="Privacy: 100% local" src="https://img.shields.io/badge/privacy-100%25%20local-ff9f0a">
</p>

---

## Overview

Image Toolkit is a free, open source web app for everyday image work. It is a single HTML file with no build step and no dependencies. Everything runs inside your browser using the Canvas and File APIs, so your images never leave your device.

The interface is designed in the style of apple.com: a clean grid of tools on the home screen, a full-screen workspace for each tool, and automatic light and dark mode.

## Tools

| Tool | What it does |
| --- | --- |
| **Convert** | Convert between PNG, JPG, WEBP, BMP and ICO. Batch conversion with ZIP download. |
| **Compress** | Compress JPG or WEBP by quality number, or type the exact file size you want in KB or MB. JPG can match the target to the byte. |
| **Resize** | Exact size, scale by percentage, or fit inside a box with optional letterbox. Single or batch. |
| **Crop** | Drag a crop box with handles, use ratio presets (1:1, 4:5, 16:9, 3:2, 9:16), or type exact X, Y, width and height. |
| **Rotate & flip** | Rotate by 90°, 180° or 270° and mirror horizontally or vertically. Single or batch. |
| **Color** | Live-preview sliders for brightness, contrast, saturation, hue and exposure. |
| **Filters** | Grayscale, sepia, invert, vintage, warm, cool, posterize, threshold, vignette, blur and sharpen. |
| **Borders** | Add padding with a solid color or gradient, with optional rounded outer corners. |
| **Rounded corners** | Export with transparent rounded corners as PNG or WEBP. |
| **Watermark** | Add a text watermark with position, size and opacity. Single or batch. |
| **Stamp** | Place a logo or sticker on a photo with size, opacity, rotation and drag-to-position. |
| **Social presets** | One-tap sizes for Instagram, Stories, X, Facebook, LinkedIn, YouTube, Pinterest, favicons and app icons. |
| **Palette** | Extract the dominant colors, tap to copy hex codes, or export a palette image. |
| **Collage** | Combine 2 to 4 photos with layouts, gaps, rounded corners and a custom background. |
| **Increase size** | Pad a JPG or PNG with extra metadata to make the file larger (up to 50 MB). |
| **Strip metadata** | Inspect EXIF and PNG metadata, remove chosen fields (such as GPS), or wipe everything by re-encoding. |

## Getting started

1. Download `index.html`.
2. Open it in any modern browser.

That is all. There is nothing to install and nothing to build.

### Host it on GitHub Pages

1. Push the files to your repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. Save. Your site will be live at `https://<your-username>.github.io/Image-Toolkit/`.

### Upload with git

```bash
git clone https://github.com/karthikhegde25/Image-Toolkit.git
cd Image-Toolkit
# add or replace files, then:
git add .
git commit -m "Update Image Toolkit"
git push
```

## Project structure

```
Image-Toolkit/
├── index.html            # the whole app: HTML, CSS and JavaScript
├── logo.png              # project logo
├── favicon-32.png        # browser tab icon
├── apple-touch-icon.png  # home screen icon
├── LICENSE               # MIT License
└── README.md
```

## Privacy

- All processing happens locally with the Canvas and File APIs.
- No accounts, cookies, analytics or tracking.
- ZIP archives are built with a small dependency-free writer, and EXIF data is edited at the byte level.
- The only network request is the Inter typeface from Google Fonts. Remove that `<link>` and the app falls back to your system fonts.

The app also includes a Privacy Policy and Terms of Use page, linked in the footer.

## Browser support

Works in current versions of Chrome, Firefox, Safari and Edge on desktop and mobile. WEBP export depends on browser support.

## Contributing

Issues and pull requests are welcome. Because the app is a single file, it is easy to read, change and test by opening it in a browser.

## License

Released under the [MIT License](LICENSE).
