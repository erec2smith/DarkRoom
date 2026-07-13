<div align="center">

# ◐ DarkRoom

**A browser-based image editor with live filters, transforms, and one-click export.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

</div>

![DarkRoom preview](images/front.jpg)

## About

**DarkRoom** is a lightweight, dependency-free image editor that runs entirely in the browser. Drop in a photo, adjust it with real-time filters, and export the result as a PNG — no upload to any server, no account, no build step required to run it.

It was built as a front-end project to explore the HTML5 Canvas API, CSS filter composition, and a clean TypeScript architecture without any UI framework.

## Features

- **Drag & drop or click to upload** — accepts JPG, PNG, and WEBP images
- **Live adjustments** — brightness, contrast, saturation, blur, hue rotation, and sepia
- **One-click effects** — grayscale and color invert toggles
- **Transform tools** — rotate left/right and flip horizontal/vertical
- **Non-destructive editing** — reset to the original image at any time
- **Export to PNG** — save the edited image straight to your device
- **Fully responsive** — works on desktop and mobile viewports

## Tech Stack

| Layer      | Technology                          |
|------------|--------------------------------------|
| Markup     | HTML5                                |
| Styling    | CSS3 (custom properties, CSS Grid)   |
| Logic      | TypeScript, compiled/bundled to JS   |
| Rendering  | HTML5 Canvas API                     |
| Bundler    | esbuild                              |

## Project Structure

```
DarkRoom/
├── index.html
├── package.json
├── tsconfig.json
├── images/
│   └── front.jpg
├── src/
│   ├── styles/
│   │   ├── reset.css
│   │   ├── variables.css
│   │   ├── layout.css
│   │   └── controls.css
│   └── ts/
│       ├── types.ts
│       ├── filters.ts
│       ├── canvasEditor.ts
│       ├── dragDrop.ts
│       ├── download.ts
│       └── main.ts
└── dist/
    └── js/
        └── bundle.js
```

## Getting Started

### Run it instantly

No installation needed. Just open `index.html` in your browser.

### Build from source

If you want to modify the TypeScript source and rebuild the bundle:

```bash
npm install
npm run build
```

This type-checks the project with `tsc` and bundles it into `dist/js/bundle.js` using `esbuild`.

## Usage

1. Drop an image onto the canvas, or click to browse your files
2. Use the **Adjust** panel to fine-tune brightness, contrast, saturation, blur, hue, and sepia
3. Toggle **Grayscale** or **Invert** for quick effects
4. Use the **Transform** controls to rotate or flip the image
5. Click **Save image** to download the result as a PNG
6. Click **Reset** at any time to revert to the original image

## Author

**Adem Mzoughi**
Software Developer

---

<div align="center">
Made with TypeScript, HTML, and CSS.
</div>
