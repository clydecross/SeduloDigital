# Sedulo Digital — Brand Context for Claude
# SEDULO-PLAYBOOK-VERSION: 1.0

## Project Overview
Sedulo Digital is a Dallas-based boutique digital agency founded by Clyde Cross. We work directly with small business owners across Texas and the U.S. who need a real web presence but lack the time or technical knowledge to figure it out themselves. We build websites, SEO foundations, and AI tools that do actual useful work for the business. Every client works with Clyde directly, start to finish. No handoffs. No account managers. No disappearing after launch.

## Tech Stack
Next.js + Tailwind CSS. CSS custom properties in brand-tokens.css. Tailwind extension in tailwind.config.js.

## Design Tokens

```css
:root {
  --sd-black: #0A0A0A;
  --sd-ink: #141414;
  --sd-graphite: #1F1F1F;
  --sd-slate: #3A3A3A;
  --sd-ash: #6B6B6B;
  --sd-smoke: #A3A3A3;
  --sd-fog: #D6D6D6;
  --sd-cloud: #EDEDED;
  --sd-paper: #F6F6F4;
  --sd-white: #FFFFFF;
  --sd-accent: #C4A882;
  --sd-accent-deep: #8C7355;
  --sd-accent-soft: #F0E8DC;
  --sd-success: #2E7D57;
  --sd-warn: #C97A1F;
  --sd-danger: #B33A2F;
  --sd-info: #2E5B8A;
  --font-display: 'Poppins', sans-serif;
  --font-body: 'Inter', sans-serif;
  --font-mono: 'JetBrains Mono', monospace;
  --fs-display-xl: 96px;
  --fs-display-l: 72px;
  --fs-display: 56px;
  --fs-h1: 44px;
  --fs-h2: 32px;
  --fs-h3: 24px;
  --fs-h4: 20px;
  --fs-lead: 20px;
  --fs-body: 17px;
  --fs-sm: 15px;
  --fs-xs: 13px;
  --fs-eyebrow: 12px;
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 12px;
  --space-4: 16px;
  --space-6: 24px;
  --space-8: 32px;
  --space-12: 48px;
  --space-16: 64px;
  --space-24: 96px;
  --space-32: 128px;
  --radius-0: 0px;
  --radius-xs: 2px;
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 12px;
  --radius-pill: 999px;
  --shadow-0: none;
  --shadow-1: 0 1px 3px rgba(0,0,0,0.08);
  --shadow-2: 0 4px 12px rgba(0,0,0,0.10);
  --shadow-3: 0 8px 24px rgba(0,0,0,0.12);
  --ease-out: cubic-bezier(0.2, 0.7, 0.2, 1);
  --dur-fast: 120ms;
  --dur-base: 200ms;
  --dur-slow: 360ms;
  --max-w-page: 1280px;
  --max-w-prose: 68ch;
}
```

## Typography Rules
- Display: Poppins SemiBold 600 — headlines, hero text, section titles, labels with presence
- Body: Inter 400/500 — body copy, descriptions, UI labels, navigation, form fields, button text
- Mono: JetBrains Mono 400 — data displays, captions, eyebrow labels, code blocks, metadata

## Color Usage Rules
- Primary: #0A0A0A — text on light, hero backgrounds, nav backgrounds, button fills
- Paper: #F6F6F4 — default page background, card surfaces on dark sections
- Accent: #C4A882 — ONE use per screen. Primary CTAs, active states, accent links, tab indicators
- Accent Deep: #8C7355 — pressed states, on-accent text
- Neutrals: #3A3A3A through #D6D6D6 — body text, captions, hairlines, dividers
- Semantic colors: functional only, never decorative

## Section Alternation Rule
Hero opens on sd-paper. Black sections are punctuation — weighted moments only (manifesto block, featured case study, closing CTA). No more than 2 consecutive same-color sections. Closing CTA is always sd-black. Footer is always sd-black.

## Component Conventions

### Buttons
- Primary: solid sd-black, sd-paper text, 4px radius, 44px min-height, Poppins SemiBold 15px, 24px horizontal padding
- Secondary: transparent, 1px sd-black border, black text, fills black on hover
- Ghost: text-only, 1px underline, underline thickens to 2px on hover
- One primary action per surface. No gradient buttons. No shadow on buttons.

### Cards
- Default: sd-paper background, 1px sd-fog border, 6px radius, 24px padding
- Feature: same but 1px sd-black border (the black frame is the Sedulo signature)
- Never rounded corners above 6px

### Form Fields
- 2px radius, 1px sd-fog border, 44px min-height, Inter 17px
- Focus: 2px sd-black outline at 2px offset
- Error: 1px sd-danger border, sd-danger error text below field
- Labels: top-aligned, Poppins SemiBold 14px, 12px gap to input
- Success state: replace form with sd-paper block, Poppins SemiBold 24px confirmation headline
- No floating labels. No shake animations. No toast popups for errors.

### Navigation
- Desktop: 64-72px tall, transparent over hero, solid on scroll, backdrop-filter blur(12px) on scroll only
- Mobile: always solid sd-paper, 64px tall, hamburger right, full-screen overlay drawer on open
- Drawer: fade + 8px translate-y, 200ms ease-out, body lock when open

## Claude Widget Conventions
When generating any visual output inside Claude conversations for this brand:

- Load fonts via Google Fonts: https://fonts.googleapis.com/css2?family=Poppins:wght@600&family=Inter:wght@400;500&family=JetBrains+Mono:wght@400
- Use CSS custom properties from the token file — never hardcode hex values
- All containers: transparent outer background
- All text: var(--sd-black) or var(--sd-paper) depending on surface — never generic gray
- Border radius: var(--radius-md) for components, var(--radius-sm) for buttons
- Swatches must show hex value labels
- Tab navigation: always functional post-streaming via JS
- No gradients, no drop shadows, no decorative effects
- All copy inside widgets must use real brand language — no Lorem ipsum
- Loading messages must reference the brand by name
- No em dashes anywhere in any output

## Copy Rules
- Tagline: Diligent work. Purposeful growth.
- Voice: Direct, grounded, unpretentious
- Lead with transformation, not features
- Use "you" language throughout
- No em dashes. Anywhere. Ever.
- No buzzwords: passionate, leverage, optimize, innovative, cutting-edge, synergy
- Sentence case for headlines. No Title Case except proper nouns.
- Fragments are fine when they land harder than a full sentence
- Write like a real human speaking clearly. Not an agency pitching.

## Brand Voice Context
Boutique agency. Clyde Cross is the face. Relational, not transactional. Faith-driven without announcing it. Approachable expert. Straight with clients. Never oversells. The copy should feel like a trusted person speaking clearly.

## Target Audience
Small business owners in Texas and across the U.S. Skilled at their work, behind online. Built on referrals. Want someone to trust with the digital side. Non-technical. Motivated by Promise of Gain — opportunity and growth, not crisis.

## Core Offer
We build the digital foundation your business has been missing. Website, SEO, and AI tools that actually work for you.

## Three Services
1. Website Build — custom Next.js, no templates, SEO-ready from day one
2. SEO — ranks, compounds, plain-language reporting
3. AI Tools — practical automations that do real work for the business

## Motivation Driver
Promise of Gain. They're not in crisis. They're in opportunity. They want growth, efficiency, and the confidence that their business is finally showing up online the way it deserves to.

## Page Architecture

### Homepage
- Hero: Diligent work. Purposeful growth. / We build the digital foundation your business has been missing. / Website, SEO, and AI tools that actually work for you. / CTA: Book a call
- Problem: You're good at what you do. The internet should know it.
- Services: Three things. Done right. (Website Build / SEO / AI Tools)
- How it works: 01 We talk. 02 We build. 03 We grow.
- Closing CTA: Your business deserves a real digital presence. Let's build it. / CTA: Book a call

### About
- Opener: I just love building things.
- Story: Seven years in tech. One big realization.
- Faith: Colossians 3:23 — work at it with all your heart
- How I build: AI-assisted development as a craftsman's better tools
- Values: Direct / Straight / Stays in your corner / Small client list by design
- CTA: Book a call

### Services
- Opener: Three things. Done right.
- Website Build / SEO / AI Tools — each with promise, includes, not-for, results
- Pricing: inquiry-based, scoped per project
- CTA: Book a call

### Learn
- Opener: Straight talk about the digital side of your business.
- 5 categories: Website and design / SEO and search / AI for small business / Business growth / Behind the build
- CMS: Supabase headless, auto-populated by category and publish date
- CTA: Book a call

### Contact
- Opener: Let's talk about your business.
- What to expect: 30-minute call, you talk, you leave with clarity, no hard sell
- Qualifier: For business owners serious about fixing their digital presence
- Form: Name / Business email / Business name / Tell me about your business
- Success state: Thanks. I'll be in touch within one business day.
- CTA: Send it

## Do Not
- Use placeholder text in production
- Deviate from the color palette without a Playbook update
- Use fonts outside the defined type stack
- Hardcode hex values in any Claude widget output
- Use em dashes anywhere in any copy or output
- Use rounded corners above 6px on cards
- Use more than one accent moment per screen
- Write buzzwords: passionate, leverage, innovative, cutting-edge
- Generate generic copy that doesn't trace back to this Brand Foundation
