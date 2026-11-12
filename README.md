# Soroptimist International City of Riverbank

Website for Soroptimist International City of Riverbank (Riverbank, California). It's a plain HTML/CSS site with no build step, served by GitHub Pages.

## Pages

| File | Page |
|---|---|
| `index.html` | Home |
| `about.html` | Mission, history, officers |
| `programs.html` | Live Your Dream Awards, Dream It Be It, community service |
| `events.html` | Upcoming events |
| `join.html` | Membership info and FAQ |
| `donate.html` | Ways to give |
| `contact.html` | Contact form (opens the visitor's email app) |

## Filling in club details

Anything the club still needs to provide is highlighted in yellow on the site and marked in the HTML with `class="todo"`. To find them all:

```bash
grep -n 'class="todo"' *.html
```

Also replace these everywhere:

- `riverbank.soroptimist@example.org`: the club's real email address
- The Facebook link in the footer (`aria-label="Facebook`)
- The **Donate Now** button `href="#"` in `donate.html`: a PayPal / Zeffy / GiveButter link

## Photos

Add photos to `images/` and replace each `<div class="photo">…</div>` placeholder with an image, for example:

```html
<div class="photo"><img src="images/charter.jpg" alt="Club members at the charter party"></div>
```

## Editing

Every page repeats the same header and footer, so a change to the menu or footer needs to be made in each `.html` file. Colors are set at the top of `css/styles.css`.

The soft watercolor backgrounds are SVG files in `images/` (`wash-hero.svg`, `wash-band.svg`, `wash-blob.svg`, `brush.svg`, `paper.svg`).
