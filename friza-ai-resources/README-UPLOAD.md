# Friza Français — public metadata only (Blogger stays the website)

This repository is **not** another website or the PWA. It hosts reference files associated with https://frizafrancais.min.ma/.

## Upload to GitHub

1. Create a public GitHub repository called `friza-public-resources` (or reuse an existing GitHub Pages repo).
2. Upload the **contents** of this folder to the repo root (`main` branch), keeping the optional `assets/` folder intact.
3. Enable Settings → Pages → Deploy from a branch → `main` → `/(root)`.
4. Replace `USERNAME` and `REPOSITORY` with your real values in the URLs below, and verify the published URLs actually open:

```
https://USERNAME.github.io/REPOSITORY/llms.txt
https://USERNAME.github.io/REPOSITORY/llms-full.txt
https://USERNAME.github.io/REPOSITORY/site-facts.json
https://USERNAME.github.io/REPOSITORY/content-index.json
https://USERNAME.github.io/REPOSITORY/social-links.json
https://USERNAME.github.io/REPOSITORY/assets/images/social-friza-1200x630.png
```

## Blogger integration

- In Blogger **Theme → Edit HTML**, update your existing `frizaLlmsTxtUrl` / `frizaLlmsFullUrl` variables in the V7.5 theme. Do not add a second duplicate metadata block.
- In the same V7.5 theme, set the existing `frizaDefaultSocialImage` to the published image URL if you want it to be your homepage sharing image. Make sure the final image URL is HTTPS, public, and returns an image response.
- Social thumbnails for **individual posts** should come from their own post images when available.

## NOT GitHub files for the Blogger domain

- `robots.txt`: configure on **Blogger → Settings → Crawlers and indexing**, not in this GitHub repo.
- `ads.txt`: configure on **Blogger → Settings → Monetization**, if you use approved advertising.
- `sitemap.xml`: use Blogger's sitemap at https://frizafrancais.min.ma/sitemap.xml; submit it to Search Console.
- `manifest.webmanifest` / `sw.js`: a service worker on github.io cannot control the Blogger origin. They are purposely not included.

## SEO limitations

`llms.txt`, other JSON resources, and GitHub links are optional supporting information and not Google ranking requirements. Keep the Blogger site as the canonical source of lesson content. The Github Pages resource index is marked `noindex` so it does not compete with the primary Blogger site.

## Content disclaimer

Category links refer to Blogger labels and may be empty until posts are published. Do not present example or unpublished lessons as published content. Verify that privacy and contact pages exist at the linked paths.
