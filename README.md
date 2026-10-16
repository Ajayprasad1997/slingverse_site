# Slingverse — Next.js IT Solutions Landing Page

## Requirements
Node.js 20+ and npm.

## Setup
```bash
npm install
npm run dev
```
Open http://localhost:3000.

## Production check
```bash
npm run typecheck
npm run build
npm start
```

## Branding
The bundled `public/logos/slingverse.svg` is an original **placeholder**, not the official logo. Replace it with your latest logo (or update `Logo` in `src/components/Landing.tsx`).

## Enquiries — important
The contact form has client and server-side validation. `src/app/api/enquiry/route.ts` intentionally returns HTTP 503 until an email provider or CRM and abuse protection are configured. It does not claim success or collect/store leads without delivery. Add your provider's **server-side** API integration, rate limiting and spam prevention before launch. The fallback is `contact@slingverse.in`.

## Content & launch
Edit `src/data/content.ts` for service text, technology and FAQs. Dashboard numbers are labeled sample data; no real client logos, unverified claims or fabricated prices are shown. Update the canonical domain in layout, sitemap and robots if deployment uses a different URL.

## Structure
`src/components/Landing.tsx`: responsive sections, scroll navigation, FAQ, animations and dashboard. `src/components/ContactForm.tsx`: validated enquiry form. `src/data/content.ts`: content arrays. `src/app`: metadata, styles, sitemap, robots and API.
