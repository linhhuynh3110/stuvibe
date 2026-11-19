# Stuvibe 🎓

**Smart vibes. Better deals.** A responsive student marketplace where university students can buy and sell second-hand items on campus: textbooks, clothing, electronics, furniture and transport.

Built with plain **HTML, CSS and JavaScript**. There's no framework and no build step.

**Live site:** [linhhuynh3110.github.io/stuvibe](https://linhhuynh3110.github.io/stuvibe/)

> Built for COIT20268 *Responsive Web Design* (CQUniversity, 2026).

---

## Features

| Page | What you can do |
|---|---|
| **Home** (`homepage.html`) | Search by name and category, browse categories, see items posted in the last 24 hours and post your own item |
| **Listings** (`listings.html`) | Filter by category, size and location; sort by price or name |
| **Product detail** (`product-detail.html`) | See price, condition, pickup location, seller reviews and similar items; chat with the seller or make an offer |
| **Saved** (`saved.html`) | Keep a list of favourite items |
| **How it works** (`how-it-works.html`) | Three steps: verify, browse, connect safely |
| **Contact** (`contact.html`) | Send a message, with live form checks and a confirmation pop-up |
| **Safety tips, Community rules, Privacy policy** | Guidance for safe, respectful trading |

### Highlights
- **Post an item:** new listings are saved in the browser and show up in the listings straight away.
- **Favourites:** tap the heart on any card to save it; saved items stay after a page reload.
- **Chat and offer pop-ups:** "Chat with seller" and "Make an offer" open accessible dialogs that keep keyboard focus inside them.
- **Live form checks:** the contact form checks name, phone, age and email as you type and when you leave each field.
- **Campus safety:** verified university-email accounts, suggested on-campus meeting spots and safety tips.

## Responsive design

The layout adapts at several breakpoints (1024, 960, 860, 768 and 560 px):

- Category and product grids go from several columns down to one.
- The navigation bar turns into a hamburger menu on small screens.
- Headings scale smoothly with `clamp()`, and containers use `min()` widths.

## Accessibility

- Semantic HTML with labelled form fields
- `aria-label`, `aria-expanded` and `aria-controls` on interactive controls
- `aria-live` regions so screen readers announce status updates
- Pop-ups that trap keyboard focus and close with Esc

## Tech stack

- **HTML5** and **CSS3** (custom properties, Flexbox, Grid, media queries)
- **Vanilla JavaScript** for search, filtering, favourites, listings and form validation
- **localStorage** for favourites (`stuvibe-favourites`) and posted items
- [Nunito](https://fonts.google.com/specimen/Nunito) from Google Fonts and [Font Awesome 6](https://fontawesome.com/) icons

## Getting started

No install needed.

```bash
git clone https://github.com/linhhuynh3110/stuvibe.git
cd stuvibe
open index.html          # or double-click it
```

`index.html` sends you straight to `homepage.html`. To run a local server instead:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Project structure

```
├─ index.html              redirects to homepage.html
├─ homepage.html           hero search, categories, new items, post an item
├─ listings.html           browse, filter and sort
├─ product-detail.html     item details, chat and offer dialogs, reviews
├─ saved.html              favourites
├─ how-it-works.html
├─ contact.html            contact form with validation
├─ safety-tips.html
├─ community-rules.html
├─ privacy-policy.html
├─ nav.css                 shared navigation styles
├─ site.css                shared site styles
└─ *.png / *.jpeg / *.webp category and banner images
```

## Design

| Colour | Hex | Used for |
|---|---|---|
| Deep green | `#08351F` | Hero overlay, dark text areas |
| Green | `#1F7A46` | Primary buttons and links |
| Light green | `#E9F8EF` | Section backgrounds |
| Yellow | `#F5C544` | Highlights and calls to action |
| Soft yellow | `#FFEBAD` | Hero heading |

## Limitations

- It's a front-end prototype with no backend. Sign-up, email verification, chat and offers are simulated.
- Posted items and favourites are stored in your browser only and don't sync between devices.

## Author

**Linh Huynh**, Master of Business Information Systems, CQUniversity Melbourne · [GitHub](https://github.com/linhhuynh3110)
