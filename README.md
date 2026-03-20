# CloudBridge Networks Website

Marketing website for CloudBridge Networks, focused on network infrastructure deployment across Africa.

Built with Astro and custom component-driven sections.

## Overview

This site is positioned as a launched technology company, not a waitlist product.

Current direction:
- Infrastructure-first messaging
- Professional B2B CTAs (Contact / Partner)
- Mobile-first responsive design
- Smooth section reveal on scroll
- Professional pricing cards and interactive pricing calculator

## Tech Stack

- Astro 6
- Plain Astro components and global CSS
- No frontend framework dependency

## Requirements

- Node.js >= 22.12.0
- npm

## Project Structure

```text
/
├── public/
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── Features.astro
│   │   ├── Pricing.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   └── pages/
│       ├── index.astro
│       ├── about.astro
│       ├── contact.astro
│       └── join-waitlist.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## Routes

- / : Home page
- /about : Company mission and vision
- /contact : Contact and partnership inquiries
- /join-waitlist : Repurposed launch/partnership page (legacy route retained)

## Development

Run from project root:

```sh
npm install
npm run dev
```

Local dev server:
- http://localhost:4321

## Build and Preview

```sh
npm run build
npm run preview
```

## Available Scripts

| Command | Description |
| :-- | :-- |
| npm run dev | Start local Astro dev server |
| npm run build | Build production output to dist |
| npm run preview | Preview production build locally |
| npm run astro | Run Astro CLI commands |

## UX and Design Notes

- Home hero uses an external Starlink-related image and professional feature cards
- Waitlist CTAs were replaced with Contact-based value CTAs
- Pricing cards were compacted for better readability and executive presentation
- Pricing calculator includes:
	- quick revenue presets
	- live plan comparison
	- best-plan recommendation and savings hint
- Theme toggle UI was removed for a cleaner professional look
- System color preference support is handled globally

## Content Maintenance

Main files to update when changing messaging:
- src/components/Hero.astro
- src/components/Features.astro
- src/components/Pricing.astro
- src/pages/about.astro
- src/pages/contact.astro

## Deployment

This project currently uses Astro default configuration.

If deploying to Netlify, Vercel, or Cloudflare Pages, use their Astro build preset with:
- Build command: npm run build
- Output directory: dist
