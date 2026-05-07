# Component System — Sedulo Digital

## Button Variants

| Variant | Background | Text | Border | Hover | Use |
|---|---|---|---|---|---|
| Primary | --sd-black | --sd-paper | none | --sd-graphite | Main CTAs — one per surface |
| Secondary | transparent | --sd-black | 1px --sd-black | bg --sd-black, text --sd-paper | Supporting actions |
| Ghost | transparent | --sd-black | none, 1px underline bottom | underline thickens to 2px | Inline links acting as CTAs |

All buttons:
- Border radius: --radius-sm (4px)
- Min height: 44px
- Horizontal padding: --space-6 (24px)
- Font: Poppins SemiBold, 15px
- Press state: scale(0.98)
- Transition: all var(--dur-fast) var(--ease-out)
- No gradient buttons. No shadow on buttons. No pill-shaped primary buttons.

## Card

Default card:
- Background: --sd-paper
- Border: 1px solid --sd-fog
- Border radius: --radius-md (6px)
- Padding: --space-6 to --space-8 (24-32px)
- Shadow: none

Feature card (the Sedulo signature):
- Same as default but border: 1px solid --sd-black
- The black frame is the elevation cue — no shadow needed

Dense card (dark surfaces):
- Background: --sd-ink
- Text: --sd-paper
- Border radius: 0
- No shadow
- Used for the most important callout on a dark section

Hover: shadow-1 (0 1px 3px rgba(0,0,0,0.08)) on default cards only
Transition: box-shadow var(--dur-base) var(--ease-out)

## Form Field

- Background: --sd-paper
- Border default: 1px solid --sd-fog
- Border radius: --radius-xs (2px)
- Min height: 44px
- Padding: --space-4 (16px) horizontal
- Font: Inter 17px, --sd-slate
- Placeholder: --sd-smoke

Focus state:
- Border: 1px solid --sd-black
- Outline: 2px solid --sd-black at 2px offset (global focus-visible rule)

Error state:
- Border: 1px solid --sd-danger
- Error text: 13px Inter, --sd-danger, 8px below input
- Form-level error banner: 1px --sd-danger border, --sd-danger summary text at top

Label:
- Font: Poppins SemiBold 14px
- Color: --sd-black
- Position: above input, 12px gap
- Required marker: asterisk inline, --sd-danger color

Success state (form level):
- Replace form with sd-paper block
- Poppins SemiBold 24px confirmation headline
- 17px Inter confirmation body
- No checkmark icon, no celebration

## Navigation

Desktop:
- Height: 64-72px
- Logo: left-aligned
- Links: right-aligned, Inter 500 15px, --sd-black
- Transparent over hero, solid on scroll
- Backdrop-filter: blur(12px) once detached from hero (only sanctioned blur)
- Active link: 2px bottom border --sd-accent

Mobile (<=768px):
- Height: 64px (never shrinks)
- Logo: left, hamburger: right
- Always solid --sd-paper, 1px --sd-fog bottom border
- No blur on mobile ever

Mobile drawer:
- Full-screen overlay, not side-slide
- Background: --sd-paper, full opacity
- Animation: fade + 8px translate-y from top, 200ms --ease-out
- Links: Poppins SemiBold 32px, left-aligned, 24px gap
- Primary CTA pinned to bottom, full-width
- Body lock: overflow hidden on open

## Section Container

- Max width: 1280px centered (--max-w-page)
- Horizontal padding: --space-6 mobile, --space-16 desktop
- Vertical padding: --space-24 to --space-32 per section (96-128px)

## Badge / Tag

- Border radius: --radius-pill (999px)
- Font: Inter 13px, weight 500
- Padding: --space-1 vertical, --space-4 horizontal
- Fills: --sd-black, --sd-paper, --sd-accent-soft
- Text on black badge: --sd-paper
- Text on paper badge: --sd-slate, with 1px --sd-fog border
- Text on accent-soft badge: --sd-accent-deep
- Never colored badges (no red, blue, green badges)

## Alert / Callout

- Border-left: 3px solid (semantic color)
- Background: semantic soft variant
- Padding: 14-18px
- Title: Poppins SemiBold 14px, semantic color
- Body: Inter 14px, semantic color
- No icons in alerts

## Naming Conventions
- Components: PascalCase (Button, Card, FormField, NavBar, SectionContainer, Badge, Alert)
- Variants: hyphen (button-primary, button-ghost, card-feature, card-dense)
- States: double-hyphen suffix (button-primary--hover, form-field--error, form-field--focus)
