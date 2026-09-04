# Bangkok Tour

A small HTML, CSS, and Pug practice project for a Bangkok tour page. The page includes tour cards, popular activities, hidden gems, a responsive footer, and social links.

## Project Structure

```text
images/                 # Page images and icons
sass/main.scss          # Sass entry file
styles/                 # Compiled CSS files
views/index.pug         # Main Pug entry file
views/mixins.pug        # Reusable Pug mixins
views/home/             # Home page sections
views/layouts/          # Header, footer, and page layout
```

## Requirements

- Node.js and npm
- Sass
- Pug CLI

Install the local development dependencies from the project root:

```bash
npm install --save-dev pug-cli sass
```

Global installation is not required. Use `npx` so the commands work without administrator permissions.

## Compile Pug

Compile the main view to HTML:

```bash
npx pug ./views/index.pug --out ./views
```

Watch the Pug files and compile automatically:

```bash
npx pug ./views/index.pug --watch --out ./views
```

## Compile Sass

Compile the Sass entry file into CSS:

```bash
npx sass ./sass/main.scss ./styles/main.css
```

Watch Sass changes:

```bash
npx sass --watch ./sass/main.scss:./styles/main.css
```

Open `views/index.html` with Live Server or the VS Code Live Preview extension after compiling.

## Image Optimization

The image files are kept locally in `images/`. For smaller page sizes, convert large JPG files to WebP with a tool such as [Squoosh](https://squoosh.app/), then update the image paths in the Pug files.
