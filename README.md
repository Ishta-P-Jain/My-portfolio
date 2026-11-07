# Ishta P Jain | Portfolio

Live : https://myportfolio-alpha-eosin-27.vercel.app/

A pastel, playful personal portfolio built with plain HTML, CSS and a little JavaScript. No frameworks and no build step, so you can open it straight in a browser.

## Features

- Pastel "sticker" design with floating shapes and a bouncy pop-in animation as you scroll
- Light and dark mode toggle (remembers your choice and follows your system setting the first time)
- Sections: Hero, About, Experience timeline, Education, Skills, Projects, Achievements, Contact
- Contact form (works with Formspree, with an email fallback until you set it up)
- Downloadable resume button
- Responsive layout with a mobile menu
- Respects the "reduce motion" accessibility setting

## Project structure

```
portfolio/
├── index.html                 # page content and the small script (theme, menu, animations, form)
├── style.css                  # all styling (colours, layout, animations, dark mode)
├── Ishta_P_Jain_Resume.pdf    # you need to add this file (see Setup)
└── README.md
```

## Setup

### 1. Add your resume
Export your resume from Overleaf and save it in this folder as `Ishta_P_Jain_Resume.pdf`. The "Download resume" button links to this exact name.

### 2. Turn on the contact form
1. Create a free form at [formspree.io](https://formspree.io).
2. Copy the form ID (the part after `/f/` in the form URL).
3. In `index.html`, find this line near the bottom and replace the placeholder:

   ```js
   var FORMSPREE_ID = "YOUR_FORM_ID";
   ```

Until you do this, the form opens your email app with the message filled in, so no messages are lost.

### 3. Check your project details
The NIWE Wind Stations bullets are drafts. Edit them in `index.html` (search for `NIWE Wind Stations`) so they describe what you actually built.

## Run locally

Open `index.html` in your browser. Or, to preview it like a real site:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy

### GitHub Pages
1. Create a repository (naming it `Ishta-P-Jain.github.io` gives you the address `https://ishta-p-jain.github.io`).
2. Upload `index.html`, `style.css`, `Ishta_P_Jain_Resume.pdf` and `README.md`.
3. Go to **Settings, then Pages**, choose the `main` branch and the root folder, and save.

### Vercel or Netlify
Import the repository, leave the build command empty, and set the output directory to the project root.

## Customising

- **Colours:** change the variables at the top of `style.css`. `:root` is light mode and `[data-theme="dark"]` is dark mode.
- **Fonts:** headings use Fredoka and body text uses Nunito, loaded from Google Fonts in `index.html`.
- **Content:** all text lives in `index.html`. Each section has a comment such as `<!-- PROJECTS -->` to help you find it.
- **Photo or screenshots:** add images to the folder and reference them from `index.html`.

## Built with

HTML5, CSS3 (custom properties, grid, flexbox) and vanilla JavaScript.

## Contact

- Email: ishta.p.jain006@gmail.com
- LinkedIn: [linkedin.com/in/ishta-p-jain](https://www.linkedin.com/in/ishta-p-jain/)
- GitHub: [github.com/Ishta-P-Jain](https://github.com/Ishta-P-Jain)
