# Small business website concepts

Two responsive, ready-to-customize static website demos for outreach to independent businesses:

| Demo | Focus | Local path |
| --- | --- | --- |
| Morrow Coffee | Café landing page, menu tabs, hours and location | `cafe/` |
| Atelier Nine | Clothing boutique editorial page and collection filters | `boutique/` |

The root `index.html` is a portfolio page that links to both concepts. All three pages work without a build step or dependencies. The businesses, addresses, prices, hours, and copy are illustrative. The original images in `assets/` were AI generated for these demos.

## Preview locally

Open `index.html` in a browser, or run a static server from the repository root:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Adapt a template for a client

1. Duplicate `cafe/` or `boutique/` into a new project.
2. Update the business name, page title, description, copy, hours, address, and navigation.
3. Replace the example image and update its description (`alt` or `aria-label`).
4. For the café, edit the `data` object near the bottom of `cafe/index.html` to change menu items and prices.
5. For the boutique, edit the collection cards and `data-category` values in `boutique/index.html`.
6. Remove the concept banner and example-address note before delivering a client site.

The designs are static front-end concepts. They do not include checkout, ordering, reservations, or a content management system.

## GitHub Pages

In the repository settings, choose **Pages → Deploy from a branch → main → / (root)**. The portfolio page will be served at `https://USERNAME.github.io/REPOSITORY/`, with the demos at `/cafe/` and `/boutique/`.
