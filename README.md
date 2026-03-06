# Luminary Studio — Static Website

A clean, responsive multi-page static website built with pure HTML and CSS. No frameworks, no dependencies, no build tools — just open and run.

---

## 📄 Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero section, services grid, stats bar, testimonial |
| About | `about.html` | Studio story, values, team cards, milestone timeline |
| Contact | `contact.html` | Contact form, office details, FAQ section |

---

## 🚀 Getting Started

No installation required. Clone the repo and open the homepage in your browser.

```bash
git clone https://github.com/your-username/luminary-studio.git
cd luminary-studio
open index.html
```

Or simply download the ZIP and double-click `index.html`.

---

## 🗂 Project Structure

```
luminary-studio/
├── index.html           # Homepage
├── about.html           # About page
├── contact.html         # Contact page
├── css/
│   ├── index.css        # Styles for homepage
│   ├── about.css        # Styles for about page
│   ├── contact.css      # Styles for contact page
│   └── main.css         # Combined stylesheet (all pages)
└── README.md
```

Each page has its own dedicated CSS file for modularity. All individual stylesheets are also collected into `main.css` for a single-file import option.

---

## ✨ Features

- **Multi-page navigation** — fixed navbar with active state highlighting and smooth transitions
- **Responsive layout** — CSS media queries for tablet (≤900px) and mobile (≤540px)
- **Mobile hamburger menu** — collapsible nav for small screens
- **Animated elements** — CSS-only marquee ticker, hover card effects, pulsing badge
- **Contact form** — budget selector, field validation, and a success state on submission
- **Consistent design system** — shared colour palette, typography, and footer across all pages

---

## 🎨 Design Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--ink` | `#0d0d0d` | Primary text, backgrounds |
| `--cream` | `#f5f0e8` | Page background |
| `--gold` | `#c8a96e` | Accents, labels, highlights |
| `--rust` | `#b94c2a` | Hover states, emphasis |
| `--mist` | `#e8e3d8` | Borders, subtle backgrounds |

**Fonts** (loaded via Google Fonts):
- [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) — headings & display text
- [DM Sans](https://fonts.google.com/specimen/DM+Sans) — body copy & UI

---

## 🌐 Browser Support

Tested and working in all modern browsers:

- Chrome / Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile Safari & Chrome for Android

---

## 🛠 Customisation

### Change the brand name
Search and replace `Luminary` across all three HTML files and in `css/main.css`.

### Update colours
CSS custom properties are declared at the top of `css/main.css`:

```css
:root {
  --ink:   #0d0d0d;
  --cream: #f5f0e8;
  --gold:  #c8a96e;
  --rust:  #b94c2a;
  --mist:  #e8e3d8;
}
```

Edit these values once in `main.css` to retheme the entire site in seconds.

### Add a new page
1. Copy any existing HTML file as a starting point
2. Create a matching CSS file in the `css/` folder (e.g. `css/newpage.css`)
3. Link it in the new HTML file: `<link rel="stylesheet" href="css/newpage.css">`
4. Update the `<title>` tag
5. Set the correct `active` class on the matching nav link
6. Update the breadcrumb in `.page-hero`
7. Optionally add the new styles to `main.css`

---

## 📦 Deployment

This site is fully static and can be deployed anywhere:

- **GitHub Pages** — push to a `gh-pages` branch or enable Pages from `main`
- **Netlify** — drag and drop the project folder at [netlify.com/drop](https://netlify.com/drop)
- **Vercel** — import the repo and deploy with zero configuration
- **Any web host** — upload the HTML files and the `css/` folder via FTP

---

## 📝 License

MIT — free to use, modify, and distribute.

---

> Built as a demonstration of a clean, production-quality static website using only HTML and CSS.
