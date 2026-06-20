# Editorial Content Search — Vue 3 + PrimeVue

A self-contained prototype of the editorial-content creation flow (Pattern D — merged catalog destination search), built with **Vue 3 + PrimeVue** loaded entirely from CDN. No build step, no dependencies to install.

## What's inside
- **App shell** — rail, topbar, and a PrimeVue `DataTable` of editorial content.
- **Create wizard** (`Dialog`) — Step 1 *Details* (BO Title, Title, sub-title, description, redirection type + CTA label) → Step 2 *Editorial content's visuals* (per-format image upload with drag & drop + alt text).
- **Pattern D search** — `SelectButton` tabs (Service / Channel / Frontspace / Catalog) with drill-down from Program → Season → Clip.

## Run locally
It's a static site — just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy to Netlify
1. Push this folder to a GitHub repository.
2. In Netlify: **Add new site → Import an existing project**, pick the repo.
3. Build settings — leave them empty:
   - **Build command:** *(none)*
   - **Publish directory:** `.` (repo root)
4. Deploy. Netlify serves `index.html` at the site root and gives you a public URL.

`netlify.toml` already pins the publish directory, so you can also drag-and-drop the folder onto the Netlify dashboard for an instant deploy.
