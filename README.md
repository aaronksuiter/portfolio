# Aaron Suiter — Portfolio

A visual portfolio website showcasing my work across **environmental science, data science, cartography, and writing**. It's a plain static website (just HTML, CSS, and images), which means it can be hosted **for free** on GitHub Pages.

**Live structure:** a home page with a thumbnail for each project; clicking a thumbnail opens a full detail page.

## Projects

| Project | Category | Detail page |
|---|---|---|
| **Manure Spotter** — peer-reviewed Google Earth Engine tool detecting manure spreading on snow | Remote sensing / data science | `manure-spotter.html` |
| **Forest Vision** — M.S. thesis on urban-forestry ecosystem-services metrics | Environmental science | `forest-vision.html` |
| **The Empire Prairie** — mapping a lost 200-sq-mile Wisconsin prairie | Cartography / environmental history | `empire-prairie.html` |
| **24 Years of Municipal Finance** — Python pipeline unifying Wisconsin financial reports | Data science | `wisconsin-policy-forum.html` |
| **The Plant Propagation Project** — blog on growing native plants from seed | Writing | `plant-propagation.html` |

## What's in this folder

```
index.html               Home page (thumbnail grid)
about.html               About page
contact.html             Contact page
manure-spotter.html      ┐
forest-vision.html       │
empire-prairie.html      ├ one detail page per project
wisconsin-policy-forum.html
plant-propagation.html   ┘
style.css                Shared styling for every page
assets/                  All images (thumbnails + full-size)
projects/                Source code, linked from the detail pages
   manure-spotter/manure_spotter.py
   wisconsin-policy-forum/Suiter_Graduate_Project.ipynb (+ data)
```

---

## How to publish it for free with GitHub Pages

You don't need to know how to code for this. There are two ways—pick whichever feels easier.

### Option A — the no-terminal way (upload in the browser)

1. Make a free account at **[github.com](https://github.com)** if you don't have one.
2. Click the **+** in the top-right → **New repository**.
   - **Repository name:** something like `portfolio` (your site will live at `https://YOUR-USERNAME.github.io/portfolio/`).
   - Set it to **Public**. Click **Create repository**.
3. On the new repo page, click **uploading an existing file**.
4. Open this `github_portfolio` folder on your computer, select **everything inside it** (the `.html` files, `style.css`, and the `assets` and `projects` folders), and drag it all into the browser upload box. Wait for it to finish, then click **Commit changes**.
5. Go to the repo's **Settings → Pages** (left sidebar).
6. Under **Build and deployment → Source**, choose **Deploy from a branch**. Set the branch to **`main`** and the folder to **`/ (root)`**, then click **Save**.
7. Wait 1–2 minutes, then refresh. GitHub will show a green banner with your live link, e.g. **`https://YOUR-USERNAME.github.io/portfolio/`**. That's your portfolio—share that link.

> Tip: to make the URL just `https://YOUR-USERNAME.github.io/` (no `/portfolio`), name the repository exactly `YOUR-USERNAME.github.io`.

### Option B — using git in a terminal

```bash
cd github_portfolio
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/portfolio.git
git push -u origin main
```

Then follow steps 5–7 above to turn on GitHub Pages.

---

## Editing it later

Every page is a normal text file you can open in any editor. To change wording, edit the relevant `.html` file. To change the look (colors, fonts, spacing), edit `style.css`—the colors are defined at the very top. To swap an image, drop a new file into `assets/` and update the `src="..."` in the page.

A few spots you may want to personalize:
- **Contact page** (`contact.html`): add your LinkedIn, GitHub, or résumé links, and the DOI/journal link for the manure paper once it's live.
- **About page** (`about.html`): tweak the bio to match how you'd describe yourself.
