# Conic — AI Employee Onboarding SaaS Landing Page

## Overview
An editorial-quality SaaS landing page for Conic, an AI-powered employee onboarding platform. Built with React, TypeScript, Tailwind CSS. Uses Instrument Serif (400) for headings and Inter (400) for body text. Framer-level polish throughout.

## Architecture
- **Frontend**: React + TypeScript + Vite, single-page with smooth-scroll navigation
- **Backend**: Express.js (minimal, serves static content)
- **Styling**: Tailwind CSS with custom CSS variables, Google Fonts (Instrument Serif + Inter)

## Pages
- `/` — Home page (`client/src/pages/home.tsx`) — full landing page with all sections

## Sections
1. **Navigation** — sticky header with desktop + mobile menu, smooth scroll to section IDs (features, how-it-works, showcase, contact)
2. **Hero** — centered layout, badge pill, person photo with gradient fade, "Get Started" + "Contact Us" CTAs
3. **Marquee** — infinite scrolling logo strip of partner companies
4. **The Numbers** — stats section with badge, heading, video mockup, 4-column stats grid (#1, 10x, 10x, 3000+)
5. **The Builder** — split layout with Instrument Serif heading + checklist + animated BuilderCard UI mockup
6. **Platform Features** — centered heading with badge, 3x2 grid of feature cards (rounded-2xl, hover lift) on #f9f8f7 bg
7. **How It Works** — 3-step cards (01, 02, 03) each with mini visual mockups inside
8. **Bento Showcase** — 2x2 bento grid: dark AI Avatar card, AI Assistant chat mockup, Dashboard with progress bars, Smart Updates sync status
9. **Testimonials** — 3 testimonial cards with star ratings, quotes, avatar initials
10. **CTA + Contact** — centered heading + form inside a rounded card (name, company, email, roles), submit button with trust badges below
11. **Footer** — logo, description, social links (Twitter, LinkedIn, Product Hunt), legal

## Typography Spec
- **Headings**: Instrument Serif, weight 400, color #111111
- **Body**: Inter, weight 400, size 14-16px, line-height 22-26px, color #53535c

## Design Tokens
- Foreground: #111111
- Body text: #53535c
- Background: #ffffff / #f9f8f7 (alternating sections)
- Card backgrounds: #f9f8f7, #f4f4f2
- Dark card: #111111 (AI Avatar bento card)
- All animations: scroll-triggered fade-up via IntersectionObserver (FadeUp component)

## Button Style (Framer-like)
- `rounded-[10px]` (nav: `rounded-[8px]`)
- Dark buttons: `background: linear-gradient(180deg, #2a2a2a 0%, #111111 100%)`
- Shadow: `0 1px 3px rgba(0,0,0,0.12), 0 0 0 0.5px rgba(255,255,255,0.06) inset`
- Hover: `scale(1.03)`, Active: `scale(0.97)`, `transition-all duration-200`
- Secondary (light): white bg, `box-shadow: 0 0 0 1px rgba(17,17,17,0.12), 0 1px 2px rgba(0,0,0,0.05)`

## Assets
- `attached_assets/image_1772808403981.png` — Conic logo (nav h-10, footer h-8)
- `attached_assets/image_1772808593132.png` — Hero person photo (bottom gradient fade)
- `attached_assets/image_1772810219209.png` — Partner logo (Anii)
- `attached_assets/image_1772810518918.png` — Partner logo (Anii2)
- `attached_assets/image_1772810741442.png` — Partner logo (Microsoft)
- `attached_assets/image_1772810808921.png` — Partner logo (CIE)
- `attached_assets/image_1772811622573.png` — Builder avatar

## Running
`npm run dev` — starts both Express backend and Vite frontend on port 5000
