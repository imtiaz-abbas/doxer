# doxer

Docsify-powered multi-product documentation hub.

## Structure

- `/` → landing page with links to all product ideas
- `/hybrid-intraday-trading-system/` → first product docs (Docsify app)

## Local Preview

Option 1 (Node.js / npm):

```bash
npm install
npm run dev
```

Open `http://localhost:8080`.

This uses Docsify CLI (recommended for plugin behavior like Mermaid).

Option 2 (Python):

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## Add a New Product Idea

1. Create a new folder at repo root (slug style), e.g. `my-new-idea/`
2. Add:
   - `index.html` (Docsify bootstrap)
   - `README.md` (idea docs)
   - `_sidebar.md` (idea navigation)
3. Add link on root `index.html`

## Deployment

- Primary: GitHub Pages via `.github/workflows/deploy-pages.yml`
- Fallback: Vercel static deployment via `vercel.json`
