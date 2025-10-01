# Aden Landing Page

High-performance landing page built with Astro for the Aden DeFi trading platform. Optimized for speed and SEO with static generation and minimal JavaScript footprint.

## Architecture

Built on Astro's island architecture, leveraging partial hydration for optimal performance. Static assets are pre-rendered at build time, with dynamic components hydrated on-demand.

### Core Stack
- **Astro 4.12** - Static site generation with component islands
- **Tailwind CSS 3.4** - Utility-first styling with JIT compilation
- **TypeScript 5.5** - Type safety across components

### Performance Optimizations
- Route-based code splitting
- Lazy loading for images and components
- Preloading critical assets
- Minified CSS with PurgeCSS integration
- Sub-50kb initial JS bundle

## Project Structure

```
src/
├── components/          # Reusable Astro components
│   ├── Partner.astro
│   ├── SecurityPartner.astro
│   └── ExchangeSelectModal.astro
├── layouts/            # Page templates
│   └── Layout.astro
└── pages/              # File-based routing
    └── index.astro
```

## Development

Install dependencies:
```bash
npm install
```

Start dev server with HMR:
```bash
npm run dev
```

Server runs on `http://localhost:4321`

## Production Build

Build static site:
```bash
npm run build
```

Preview production build locally:
```bash
npm run preview
```

Output directory: `dist/`

## Deployment

Static output is compatible with any CDN or static host:
- Vercel
- Netlify
- Cloudflare Pages
- AWS S3 + CloudFront

Build output is fully static HTML with minimal JS hydration where needed.

## Configuration

`astro.config.mjs` - Main Astro configuration
`tailwind.config.mjs` - Tailwind customization
`tsconfig.json` - TypeScript compiler options

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

Modern browsers only. No IE11 support.
