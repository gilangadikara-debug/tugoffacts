# Studio Light Lab

A free, browser-based studio lighting simulator for photography education. Place up to eight lights with softboxes, octaboxes, beauty dishes, umbrellas, strip boxes, grids, snoots, fresnels and colour gels around a real head scan, posable male and female figures or still-life sets, and read the result on a built-in light meter.

© 2026 Gilang Adikara. Free to use, modify and distribute for educational and non-commercial purposes. See [LICENSE.md](LICENSE.md) and [CREDITS.md](CREDITS.md).

## Put it online with GitHub Pages and your own domain

1. **Replace the placeholder domain.** Search the project for `YOUR-DOMAIN` and replace it with your domain, for example `lightlab.example.id`. It appears in `index.html` (7 times), `robots.txt` and `sitemap.xml`.
2. **Create a repository** on GitHub (public), for example `studio-light-lab`, and upload every file and folder in this package to the root of the repository, including the hidden `.nojekyll` file.
3. **Turn on Pages:** repository **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. **Connect your domain:** on the same Pages screen, enter your domain under **Custom domain** and save. GitHub adds a `CNAME` file to the repository for you.
5. **Point DNS at GitHub** at your domain registrar:
   - Subdomain (e.g. `lightlab.example.id`): add a `CNAME` record from `lightlab` to `<your-github-username>.github.io`.
   - Root domain (e.g. `example.id`): add four `A` records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`.
6. Wait for DNS to take effect (minutes to a few hours), then tick **Enforce HTTPS** on the Pages screen.

## Help search and AI engines find it

- Add the site to **Google Search Console** and **Bing Webmaster Tools**, verify it, and submit `https://YOUR-DOMAIN/sitemap.xml`.
- Check the social preview with the Facebook Sharing Debugger or LinkedIn Post Inspector after the site is live.
- Links from your university profile, course pages, blog or social posts help it get discovered faster.

## What's in the package

| Path | Purpose |
|---|---|
| `index.html` | The whole app, with page title, description, social-preview tags and structured data |
| `models/` | Head scan and the two sculpted figures (binary glTF) |
| `textures/` | Skin colour and detail maps for the head scan |
| `og-image.jpg` | 1200×630 preview image used when the link is shared |
| `favicon.svg` | Browser tab icon |
| `robots.txt`, `sitemap.xml` | Tell crawlers they may index the site and where to find it |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

The app loads three.js and fonts from public CDNs, so it needs an internet connection. Your settings and captures are stored in each visitor's own browser.
