# MCP App Store · Blog redesign prototype

Two-page interactive prototype of the redesigned [MCP App Store](https://mcp-app-store.keenethics-labs.com/blog) blog, in the KeenEthics visual style.

## Live preview

- **Index page** → [index.html](./index.html)
- **Article page** → [article.html](./article.html)

Once GitHub Pages is enabled for this repo, both pages will be reachable at:

```
https://developerscompany.github.io/MCP-App-Store---Blog/
https://developerscompany.github.io/MCP-App-Store---Blog/article.html
```

## What's in the prototype

- Brand-aligned design tokens pulled from `keenethics.com` (Raleway, `#2969CC` blue, `#D62C2C` red, `#12233D` navy, 8px button radius).
- New cover system — relevant photo background + semantic icons (MCP App Store paperclip mark, real Claude 12-spoke asterisk, OpenAI knot, Cursor pointer).
- Article cards with category coding (How-to / Compare / Insight / Platform), all colors strictly from the KeenEthics palette.
- Lead-gen surfaces:
  - Sticky author rail in the article with Daria's photo, online indicator and free-review CTA.
  - Inline contextual CTAs throughout the article body.
  - Newsletter capture (The MCP Brief) with real face avatars.
  - Big bottom CTA in the corporate-blue KeenEthics layout with Daria's photo.
- Social proof bar using real KeenEthics client logos (Visa, Nokia, Epson, WorldLabs, Paystub, BankerAdvisor, Edstruments, Brainable, StoryTerrace).
- Reading progress bar + sticky TOC on the article page.
- Filter pills (How-to · Compare · Insight · Platform), search field, breadcrumb, related articles, footer.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000/index.html
```

Direct `file://` opening will not load Google Fonts due to CORS, so a local server is required.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Blog list page (hero, filters, grid, newsletter, CTA, footer). |
| `article.html` | Single article page (hero, TOC, body with inline CTAs, related, CTA). |
| `styles.css` | Shared design system (tokens + all components). |
| `daria.webp` | Daria Hlavcheva — Head of Partner Engagement, used in personalized CTAs. |
| `mcp-icon.png` | MCP App Store paperclip mark, sourced from the existing blog cover assets. |
