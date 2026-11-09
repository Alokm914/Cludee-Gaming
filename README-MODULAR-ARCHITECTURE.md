# Feature branch: modular website architecture

This branch adds an isolated module scaffold to the existing Cludee Gaming website.
The current root `index.html`, `css/style.css`, and `js/script.js` remain the main website.

## Added structure

- `modules/index.html` — development directory for independent modules
- `modules/advertising/` — advertising module scaffold
- `modules/tournaments/` — tournament module scaffold
- `modules/news/` — news and updates module scaffold
- `modules/dashboard/` — future management dashboard scaffold

Each module has its own `index.html`, `style.css`, and `script.js`.

## Preview

Open `modules/index.html` through VS Code Live Server / Live Preview.
The main website remains available from the root `index.html`.

## Git branch workflow

Run these commands from the repository root:

```bash
git switch main
git pull origin main
git switch -c feature/modular-architecture
```

Copy the added `modules/` directory and this README into the working repository, then:

```bash
git add modules README-MODULAR-ARCHITECTURE.md
git commit -m "Add independent website module scaffolds"
git push -u origin feature/modular-architecture
```

Then create a Pull Request on GitHub from `feature/modular-architecture` into `main`.
Review and test the changes before merging.

## Safety and scope

- This ZIP does not publish changes to GitHub or create a remote branch.
- No existing main-page navigation or behavior is replaced.
- The advertising module does not serve ads.
- The dashboard is only a front-end placeholder; it has no authentication.
- Do not put API keys, passwords, tokens, or private credentials in client-side files.
- Get website-owner approval before publishing ads, player data, tournament details, or dashboard functionality.
