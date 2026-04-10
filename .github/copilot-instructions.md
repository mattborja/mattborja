## Repository Overview

This is the **mattborja/mattborja** special repository. It serves two purposes:

1. **GitHub Profile**: `README.md` at root is displayed on [github.com/mattborja](https://github.com/mattborja).
2. **Personal Website**: `index.html` at root is deployed via GitHub Pages to [mattborja.dev](https://mattborja.dev).

GitHub Pages is configured to deploy from root (`/`) of the `master` branch.

## Repository Structure

```
/
├── README.md              # GitHub Profile (displayed on github.com/mattborja)
├── index.html             # Personal website homepage (mattborja.dev)
├── mattborja.min.jpg      # Profile photo (used by index.html)
├── .gitignore
└── .github/
    └── copilot-instructions.md   # This file
```

## Conventions

### Commit Messages

This project enforces **Conventional Commits** (https://www.conventionalcommits.org/).

Format: `<type>(<scope>): <description>`

**Types:**
- `feat`: New feature or content addition
- `fix`: Bug fix or correction
- `docs`: Documentation changes (README.md, comments)
- `style`: Formatting, whitespace, CSS-only changes (no logic change)
- `refactor`: Code restructuring without behavior change
- `chore`: Maintenance tasks (.gitignore, tooling, config)
- `ci`: CI/CD configuration changes

**Scopes:**
- `profile`: Changes to README.md (GitHub Profile)
- `site`: Changes to index.html or website assets (mattborja.dev)
- `repo`: Repository-level config (.gitignore, .github/, etc.)

**Examples:**
```
feat(site): add ORCiD link to social section
fix(site): correct avatar image path
docs(profile): update bio and badges
chore(repo): add deploy key to .gitignore
```

### Deployment

- **Do NOT force push to `master`** — it triggers a GitHub Pages deployment.
- Always verify changes locally before committing.
- The `deploy_key` and `deploy_key.pub` files are git-ignored and must never be committed.

### Website (index.html)

- Single-file static site (HTML + inline CSS, no external JS).
- Profile image: `mattborja.min.jpg` (referenced as relative path).
- All rights reserved — not open-source licensed.

### GitHub Profile (README.md)

- Keep concise. Badges link to LinkedIn, ORCiD, and mattborja.dev.
- Mirrors the terminal motif from the website.
