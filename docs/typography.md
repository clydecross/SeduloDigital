# Typography System — Sedulo Digital

## Font Stack
- Display: Poppins SemiBold 600 — loaded from Google Fonts: https://fonts.googleapis.com/css2?family=Poppins:wght@600
- Body: Inter 400/500 — loaded from Google Fonts: https://fonts.googleapis.com/css2?family=Inter:wght@400;500
- Mono: JetBrains Mono 400 — loaded from Google Fonts: https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400

## Usage Rules
- Display font (Poppins SemiBold): hero headlines, section titles, card titles, labels with presence, any text that needs emotional weight, button text, eyebrow labels
- Body font (Inter): all body copy, UI labels, navigation links, form fields, descriptions, list items, table cells
- Mono font (JetBrains Mono): eyebrow metadata, data displays, captions, code blocks, numbers that need precision treatment

## Type Scale

| Token | Desktop | Tablet (<=1024) | Mobile (<=768) | Use |
|---|---|---|---|---|
| --fs-display-xl | 96px | 72px | 48px | Hero headlines |
| --fs-display-l | 72px | 56px | 40px | Large section headlines |
| --fs-display | 56px | 44px | 34px | Section openers |
| --fs-h1 | 44px | 36px | 28px | Primary page headings |
| --fs-h2 | 32px | 28px | 24px | Sub-section headings |
| --fs-h3 | 24px | 22px | 20px | Card titles |
| --fs-h4 | 20px | 19px | 18px | Small headers |
| --fs-lead | 20px | 19px | 18px | Intro paragraphs |
| --fs-body | 17px | 17px | 16px | Default body |
| --fs-sm | 15px | 15px | 14px | Dense data, table cells |
| --fs-xs | 13px | 13px | 13px | Captions, footnotes |
| --fs-eyebrow | 12px | 12px | 12px | Uppercase labels |

## Line Height Rules
- Display sizes: 1.02
- Headings h1-h2: 1.1 to 1.15
- Headings h3-h4: 1.25 to 1.3
- Body and lead: 1.55
- Mono captions: 1.4

## Letter Spacing Rules
- Display sizes: -0.02em
- h1: -0.01em
- Eyebrows: 0.14em (always uppercase)
- Body: default (0)

## Weight Rules
- Poppins: always 600 (SemiBold)
- Inter: 400 for body copy, 500 for labels and button text
- JetBrains Mono: always 400

## Casing Rules
- Sentence case for almost everything
- Title Case only for proper nouns
- ALL CAPS reserved for short eyebrow labels only

## Text Wrap
- Headings: text-wrap: balance
- Body: text-wrap: pretty
- Prose max width: 68ch (--max-w-prose)
