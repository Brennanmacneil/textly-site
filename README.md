# Textly — AI iMessage assistant for car dealerships (marketing site)

A complete, responsive, deployable marketing site for an AI-powered iMessage lead-engagement
platform built for car dealerships. Self-contained: all mockups are inline SVG/CSS — **no
external image dependencies.**

## Files
| File | What it is |
|------|------------|
| `index.html` | The full landing page (nav, hero, problem, 9 features, "you're not spam" section, how it works, live dashboard, results + testimonials, pricing, FAQ, final CTA, footer). |
| `book-demo.html` | The "Book a demo" conversion page (the primary CTA destination) with a working front-end form + the live call-the-AI line. |
| `README.md` | This file. |

## Run / deploy
It's static HTML — no build step.
- **Locally:** just open `index.html` in a browser (or `python3 -m http.server` and visit it).
- **Deploy:** drop the folder on Netlify, Vercel, Cloudflare Pages, GitHub Pages, or any static host.

> Styling uses the Tailwind **CDN** + Google Fonts (Inter). That keeps the deliverable
> zero-build and copy-paste deployable. For a hardened production build, install Tailwind
> locally and compile a purged stylesheet (`npx tailwindcss -i in.css -o out.css --minify`)
> and self-host Inter — the markup is already Tailwind-class-based, so nothing else changes.

## Design direction (matches your 3 reference images)
- **Top green call-banner** ("Call Our AI: (249) 209-5699") — like your screenshot. The number
  is a `tel:` link and appears in the banner, hero, dashboard CTA, demo page, and footer.
- **Problem section** "*Unknown Caller isn't a business strategy*" with the green dialpad /
  "Calling as [dealer name]" mockup — mirrors **image 1**.
- **Dark "*You're not spam*" section** with a phone iMessage mockup over faint code — mirrors **image 2**.
- **Light dashboard** "*Every call, text, and follow-up. In one view.*" with KPI pills, a campaign
  progress card, bar charts, an AI-vs-human donut, and a live escalation list — mirrors **image 3**.
- Premium B2B SaaS: royal-blue → indigo accent (the iMessage product color), deep dealership
  green as the trust/utility color, rounded cards, generous whitespace, Inter, tasteful
  scroll-reveal motion.

## What's a placeholder (swap before launch)
- **Brand name & logo** — **Textly** (textly.ca). The logo wordmark is `Text<span>ly</span>`.
- **Phone number** `(249) 209-5699` — search/replace `+12492095699` and `(249) 209-5699`.
- **Pricing** ($1,490 / $1,990 / Custom) — set your real tiers in the Pricing section.
- **Stats & testimonials** — all illustrative; replace with your real numbers and quotes.
- **Demo form** — front-end only; wire `#demoForm` in `book-demo.html` to your CRM/backend
  (HubSpot, Salesforce, or a serverless endpoint).
- **Footer/legal links** — point to your real privacy, terms, and messaging-policy pages.

## Brand
The site is branded **Textly** (textly.ca) — the two-tone logo splits as `Text` + `ly`.
To rename later, replace `Textly` and the `Text<span...>ly</span>` wordmark across both HTML
files (and the chat-bubble logo `<svg>` if you want a different glyph).
```

🤖 Generated with [Claude Code](https://claude.com/claude-code)
