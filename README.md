# Bangkok Tour — Landing Page

landing page built with HTML. CSS through **Pug (Jade)**, **Dart Sass (SCSS)**.

![Bangkok Tour Preview](images/preview.jpg)

---

## Highlights & Features

- **Semantic HTML5 & Pug Templating:** Reusable layouts, mixins, and includes for clean, modular markup.

- **Modern Sass Architecture (Sass Module System):** Utilizes modern `@use` and `@forward` rules (Dart Sass 1.80+ standard) replacing deprecated `@import`.

- **Responsive Web Design (RWD):** Fluid typography, Flexbox, and CSS Grid layouts optimized across Mobile, Tablet, and Desktop breakpoints.

- **Micro-interactions:** Smooth CSS transitions for button states, card hover lift effects, and interactive header pills.

- **Organized Structure:** BEM naming convention and 7-1 pattern directory structure (Abstracts, Base, Components, Layouts).

---

## My Project Structure

```text
html-css-basics/
├── images/                 # Optimized photography and icons
├── sass/                   # Modern Sass (SCSS) source files
│   ├── abstracts/          # Variables, mixins, and _index.scss (@forward)
│   ├── base/               # CSS reset and global utilities
│   ├── components/         # Buttons, top tours, popular, hidden gems
│   ├── layouts/            # Header and footer styles
│   └── main.scss           # Main Sass entry point (@use modules)
├── styles/                 # Compiled CSS output and source maps
├── views/                  # Pug template files
│   ├── home/               # Section views (TopTours, Populars, HiddenGems)
│   ├── layouts/            # Base Tour-layout, Header, Footer
│   ├── mixins.pug          # Reusable Pug mixins
│   ├── index.pug           # Main page template
│   └── index.html          # Compiled HTML output
├── knowledge.md            # Master course notes and CSS cheat sheet
└── package.json            # Build scripts and dependencies
```

---

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) (v18 or newer) installed on your machine.

### Installation

Clone the repository and install the development dependencies:

```bash
git clone <repository-url>
cd html-css-basics
npm install
```

---

## Development & Build Scripts

Run these scripts from inside the `html-css-basics` directory:

| Command              | Description                                                        |
| :------------------- | :----------------------------------------------------------------- |
| `npm run sass:build` | Compiles `sass/main.scss` into `styles/main.css` (single build).   |
| `npm run sass:watch` | Watches for `.scss` changes and compiles CSS in real-time.         |
| `npm run pug:build`  | Compiles `views/index.pug` into `views/index.html` (single build). |
| `npm run pug:watch`  | Watches for `.pug` changes and compiles HTML in real-time.         |

```bash
xdg-open views/index.html
```

---

## Technologies Used

- **Markup:** [Pug](https://pugjs.org/) (formerly Jade)
- **Styling:** [Dart Sass](https://sass-lang.com/) (SCSS syntax)
- **Icons:** [Bootstrap Icons CDN](https://icons.getbootstrap.com/)
- **Typography:** [Google Fonts (Inter)](https://fonts.google.com/specimen/Inter)
- **Version Control:** Git & GitHub

---

## 📄 License

This project is open source and available under the [ISC License](LICENSE).
