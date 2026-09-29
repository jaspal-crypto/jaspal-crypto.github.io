# Jaspal Singh — academic homepage

A compact desktop academic website built with plain HTML and CSS. No build step, JavaScript, or backend is required. Charter is used for body text and Source Sans 3 for headings and navigation; both are bundled locally with their redistribution licenses. Charter includes true italic, bold, and bold italic styles.

## Preview

Open `index.html` in a browser, or run this from the site folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then visit [the local preview](http://127.0.0.1:8000/index.html). Stop the server with Control-C when finished.

## Publishing and future updates

The live site is https://jaspal-crypto.github.io/. GitHub Pages publishes directly from the `master` branch, `/(root)`, using the included `.nojekyll` file. The old Jekyll **Deploy site** workflow is disabled.

Edit the four root HTML files or `assets/styles.css` in this repository, then use GitHub Desktop to commit to `master` and **Push origin**. GitHub Pages publishes the update automatically; deployment status appears under **Actions → pages build and deployment**. No build command or dependencies are needed.

The old `/publications/` address redirects to `publications.html`. Images, fonts, and internal links use relative paths. The old Jekyll source files and legacy assets remain for reference and existing file links; they are not used to build the new site. Keep font license files with the bundled fonts.

## Editing

| File | Content |
| --- | --- |
| `index.html` | Biography, research openings, updates, portrait, and contact details |
| `research.html` | Exact supplied research descriptions and three figures |
| `publications.html` | Two preprints and fifteen selected publications |
| `teaching.html` | Course details and future slide links |
| `assets/styles.css` | Desktop layout, typography, colors, and spacing |
| `assets/images/` | Portrait, research figures, and handwritten contact image |
| `assets/fonts/` | Local fonts and licenses |
| `AGENTS.md` | Project preferences, including desktop-only design |

Copy an existing publication `<article>` to add a paper. Give the article and heading unique IDs, update the title/authors/venue, add the full original abstract inside `<details>`, and update the PDF link. Keep the paper in either Preprints or Selected Publications; there are no year sections.

Venue lines are bold. Each title ends in † for alphabetical order or ‡ for contribution order. The compact legend under Selected Publications also explains * for equal contribution. Batched DPF uses contribution order, as confirmed by the author; do not infer the convention solely from how the names sort. Keep all author names at the same weight, and use Jaspal Singh without Saini.

Copy a news `<li>` to add an update. The short news area scrolls when more entries are added. Headers are repeated across the four pages; apply navigation changes consistently.

The contact address is displayed as a handwritten image in `assets/images/contact.png`, beside the Email: label. The sidebar affiliation reads MBZUAI, UAE without a link. No email address is embedded in HTML, links, or alternative text. The image discourages simple text scraping but does not prevent OCR.

## Design

Desktop only, as requested for the entire project. A 960px content column sits inside a full-height, 1040px white central band, with very pale mauve filling the surrounding screen. Charcoal text, plum links, a mauve openings box, compact spacing, and a 140px portrait on the right. Research figures are centered beside their descriptions, at 150px for foundations and 240px for the other two directions. No mobile/tablet layouts, hero copy, year sidebars, site footers, or decorative image captions.

Update `publications.html` to change paper links. Keep all font license files in `assets/fonts/`.

## Abstract sources

The Abstract disclosures contain original full abstracts rather than summaries. Source URLs are recorded in each abstract’s `data-source` attribute. Thirteen abstracts were retrieved from IACR ePrint or Springer, and the Gauss preprint abstract from arXiv; the two older ACM/IEEE abstracts were taken from the author’s existing homepage when publisher endpoints blocked retrieval. The S&P 2027 paper has no abstract or PDF link yet. Equations are converted to static MathML, which needs no JavaScript or external service. Research prose and publication titles follow the supplied content; the 2016 graph-computation paper is marked as a poster.
