# Obsidix Landing Page — Next.js

## Stack
- **Next.js 14** (App Router)
- **TypeScript**
- **CSS Modules** (zero external dependencies)

## Setup

```bash
# 1. Install dependencies
npm install

# 2. Run dev server
npm run dev
# → http://localhost:3000

# 3. Production build
npm run build
npm start
```

## Project Structure

```
src/
├── app/
│   ├── layout.tsx       # Root layout + metadata
│   └── page.tsx         # Main page (assembles all components)
├── components/
│   ├── Navbar.tsx / .module.css
│   ├── Hero.tsx / .module.css
│   ├── AdvantageBar.tsx / .module.css
│   ├── Divisions.tsx / .module.css
│   ├── About.tsx / .module.css
│   ├── Mission.tsx / .module.css
│   ├── Compliance.tsx / .module.css
│   ├── Contact.tsx / .module.css
│   └── Footer.tsx / .module.css
└── styles/
    └── globals.css      # Design tokens + reset

public/
├── obsidix-logo.png     # Obsidix main logo
└── vuriza-logo.png      # Vuriza Shield logo
```

## Sections
1. **Navbar** — Fixed, with logo + nav links + Contact Sales CTA
2. **Hero** — Full-screen with animated logo, rings, headline
3. **AdvantageBar** — 4 pillars strip
4. **Divisions** — 4 cards (Vuriza Shield featured)
5. **About** — Company description
6. **Mission** — Statement + 3 pillars (Legal / Financial / Technological)
7. **Compliance** — GDPR text + live status panel
8. **Contact** — Contact card
9. **Footer** — Logo, legal links, address, copyright

## Notes
- Logos use `mix-blend-mode: lighten` so black backgrounds are invisible
- All animations defined in `globals.css` keyframes
- Fully responsive (mobile breakpoints in each module)
