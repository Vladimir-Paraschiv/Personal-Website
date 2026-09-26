# Vladimir Paraschiv — Personal Portfolio

A responsive, interactive portfolio built with plain HTML, CSS, and JavaScript. No framework, npm install, backend, or build step is required.

## Files

- `index.html` — page structure, profile, project cards, résumé section, and contact dialog.
- `style.css` — light/dark themes, responsive layouts, and animations.
- `app.js` — section switching, project details, theme preference, and contact interactions.
- `portrait.jpg` — original portrait used by the current site.
- `resume.pdf` — downloadable résumé.
- `.nojekyll` — tells GitHub Pages to serve the files directly.

## Run locally

Extract this ZIP and open a terminal inside the `vladimir-portfolio` folder.

With Python installed:

```bash
python -m http.server 8000
```

On systems where Python is named `python3`, use `python3 -m http.server 8000`. Then visit http://localhost:8000. Stop the server with Ctrl+C.

Alternatively, open the folder in VS Code and serve `index.html` using Live Server.

## Edit the site

- Change visible profile text and project-card labels in `index.html`.
- Change project descriptions, repository URLs, and live-demo URLs in the `projects` object near the beginning of `app.js`.
- When changing a project name or technologies, update both its HTML card and JavaScript detail record.
- Change colors using the CSS variables in `:root` and `body.light` in `style.css`.
- Replace `portrait.jpg` or `resume.pdf` while keeping the filenames, or update their references in `index.html`.
- Contact email appears in both `index.html` and `app.js`; update all occurrences when changing it.

## Included interactions

- Projects, About, and Résumé panels with animated transitions.
- Project dialogs with Overview, How it works, Demo, and Code tabs.
- Light/dark preference stored locally in the visitor's browser.
- LinkedIn and GitHub links.
- Contact dialog with Copy email, Open Gmail, and Open Outlook.
- Clipboard fallback that selects the email address for manual copying.
- Keyboard-friendly native dialogs and reduced-motion support.

## Current limitations

- The portrait retains its original background; background removal was not successful.
- E-Commerce has a linked live demo. Medicine Management requires its separate Express backend; see its repository instructions. The voting capstone has no linked public repository or demo yet. The repository is managed by a separate group member.
- This portfolio does not host the project backends or send email itself. Gmail and Outlook links open webmail and may require sign-in.
- Google Fonts needs an internet connection; the CSS includes fallback fonts.
- Automatic clipboard access depends on browser permissions and a secure context (HTTPS or localhost). Manual copying remains available.
- `resume.pdf` is included as provided; its GitHub text may still show the previous username.
