# Jonny Ross — Personal Website

Two self-contained static HTML files. No build step, no dependencies — fonts, scripts, portrait and company logos are all embedded, so they work offline and on any static host.

- `index.html` — home (hero, about, experience accordions, testimonials, contact)
- `tools.html` — tools & proficiency ratings

Both share a viewer-selectable design theme (Startup / Scaleup / Enterprise).

---

## Host on GitHub Pages

1. **Upload the files.** In your repo (`github.com/jonnyiross-creator/profile`): **Add file → Upload files** → drag in `index.html` and `tools.html` (they must sit at the repo root) → **Commit changes**.
2. **Enable Pages.** Repo **Settings → Pages** → Source = **Deploy from a branch** → Branch = **main**, folder = **/ (root)** → **Save**.
3. **Wait ~1 minute.** The live URL appears at the top of the Pages settings page:
   `https://jonnyiross-creator.github.io/profile/`

The Tools link works automatically (relative `tools.html`).

## Host on Vercel (alternative)

[vercel.com](https://vercel.com) → **Add New → Project** → **Import** the `profile` repo → Framework preset **Other** (no build command, output dir = root) → **Deploy**. You get a URL like `profile.vercel.app`.

> Use one host, not both.

---

## Updating the site

Re-upload the new `index.html` / `tools.html` (or `git push`) — the host redeploys automatically in ~1 minute.

These files are **compiled output**. The editable source lives in the design project; make real changes there and re-export, rather than hand-editing these files. Small one-line typo fixes directly here are fine.

## Custom domain

Once you own a domain, add it under **Settings → Pages → Custom domain** (GitHub) or the **Domains** tab (Vercel) and follow the DNS records they show.
