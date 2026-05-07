# Color System — Sedulo Digital

## Brand Colors

| Name | Token | Hex | Role | Use |
|---|---|---|---|---|
| Black | --sd-black | #0A0A0A | Primary | Text on light, hero backgrounds, nav backgrounds, button fills, feature card borders |
| Ink | --sd-ink | #141414 | Dark surface | Dark mode surfaces |
| Graphite | --sd-graphite | #1F1F1F | Elevated dark | Button hover state on dark |
| Paper | --sd-paper | #F6F6F4 | Page background | Default page background, card surfaces on dark sections, form backgrounds |
| White | --sd-white | #FFFFFF | Pure white | Component backgrounds where maximum contrast needed |
| Dusty Gold | --sd-accent | #C4A882 | Accent — 1 per screen | Primary CTA fill, active tab indicator, accent links, single highlighted element |
| Dusty Gold Deep | --sd-accent-deep | #8C7355 | Pressed / on-accent | Pressed state on accent elements, text on accent backgrounds |
| Dusty Gold Soft | --sd-accent-soft | #F0E8DC | Tinted background | Accent state backgrounds, badge fills |

## Neutrals

| Name | Token | Hex | Use |
|---|---|---|---|
| Slate | --sd-slate | #3A3A3A | Body text on light surfaces |
| Ash | --sd-ash | #6B6B6B | Metadata, captions, secondary labels |
| Smoke | --sd-smoke | #A3A3A3 | Placeholder text, disabled states |
| Fog | --sd-fog | #D6D6D6 | Hairlines, dividers, default borders |
| Cloud | --sd-cloud | #EDEDED | Soft fills, hover states on light |

## Semantic Colors (functional only — never decorative)

| Token | Hex | Use |
|---|---|---|
| --sd-success | #2E7D57 | Form submission confirmation, completed steps |
| --sd-warn | #C97A1F | Availability notices, timeline alerts |
| --sd-danger | #B33A2F | Form errors, invalid input, destructive actions |
| --sd-info | #2E5B8A | Helper notes, neutral informational callouts |

## Section Alternation Rule
Marketing pages alternate between sd-paper and sd-black sections. Hero opens on sd-paper. Black sections are weighted moments only. No more than 2 consecutive same-color sections. Closing CTA is always sd-black. Footer is always sd-black. Hard edges between sections — no gradient transitions.

## Pairing Rules
- sd-black on sd-paper: primary text treatment, always legible
- sd-paper on sd-black: inverted sections, hero text on dark backgrounds
- sd-accent on sd-black: the one warm moment on dark surfaces
- sd-accent on sd-paper: primary CTA treatment on light backgrounds
- sd-slate on sd-paper: body copy on light backgrounds
- Never pair sd-accent-soft as a section background color

## Accent Usage Rule
One accent moment per screen. Maximum. This applies across the entire viewport at any given scroll position. The accent is punctuation — it marks the single most important interactive or informational element. When everything is accented, nothing is.

## Dark Mode
Token swap only — no component-level changes needed.
- bg becomes sd-black
- text becomes sd-paper
- border-strong becomes 1px sd-paper (inverted)
- focus-ring uses sd-accent on dark (the one place accent leads)
