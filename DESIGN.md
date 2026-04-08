# Design System Inspiration of Lenovo

## 1. Visual Theme & Atmosphere

Lenovo's design language is built on a single, unwavering conviction: **one red rules everything**. Signature Red (`#E2232A`) is not an accent — it is the brand's heartbeat, present in every communication and used to draw the eye to what matters most. Everything else retreats to black, white, and neutral grays, creating a stage on which that red can perform.

The overall atmosphere is **bold precision meeting human warmth**. Helvetica Neue provides the architectural backbone — rational, international, trustworthy. But Lenovo softens the pure corporate edge through its history of building machines for real people: the typography stays tight and confident but never cold. White space is used generously, not as decoration but as breath between statements.

The OneLenovo evolution adds a secondary dimension: a **Deep Purple** (`#4D144A`) that acts as a "harmonious companion" to Red — adding richness and premium depth without competing. Together they create a palette that is distinctly Lenovo and unlike any other tech brand.

**Key Characteristics:**
- Signature Red as the single dominant interactive and brand color
- Helvetica Neue with tight 95% headline leading — "engineered confidence"
- White and near-white backgrounds as the primary canvas
- L-pattern texture: repeating the "L" letterform creates ownable graphic texture
- Flat, clean surfaces — depth through color contrast, not shadow
- Product-hero photography on white fields with generous breathing room
- Red as typographic punctuation: headlines, CTAs, underlines, rule lines

## 2. Color Palette & Roles

### Primary Brand
- **Signature Red** (`#E2232A`): The singular brand color — CTAs, logo, active states, brand moments
- **Black** (`#000000`): Primary text, hero backgrounds, dominant statements
- **White** (`#FFFFFF`): Page backgrounds, card surfaces, negative space

### Neutral System
- **Charcoal Gray** (`#6F7170`): Secondary body text, metadata, captions
- **Light Warm Gray** (`#C4BEB6`): Dividers, disabled states, subtle borders
- **Off White** (`#D9D8D6`): Alternate section backgrounds, input fields
- **Near Black** (`#1A1A1A`): Primary body text on light backgrounds

### OneLenovo Accent System
- **Deep Purple** (`#4D144A`): Premium accent, section highlights, brand moments alongside Red
- **Deep Red** (`#64131E`): Hover/pressed state for Signature Red, dark hero overlays
- **Mid Coral** (`#F26A52`): Warm gradient companion, data visualization, secondary highlights
- **Mid Salmon** (`#FFB9A2`): Tinted illustrations, soft data bars

### Tint Palette (Backgrounds & States)
- **Pale Red** (`#FAECEB`): Error states, alert backgrounds, light brand tint sections
- **Pale Red Mid** (`#F0C7BF`): Hover tint on red interactive elements
- **Pale Purple** (`#F1E1ED`): Premium feature callout backgrounds
- **Pale Purple Mid** (`#D9C1D8`): Purple tint section backgrounds
- **Pale Blue** (`#EAEEF5`): Neutral informational callouts
- **Pale Blue Mid** (`#C9D0F0`): Table row alternates, subtle data backgrounds

### Semantic
- **Error / Danger**: Signature Red (`#E2232A`) — Red already serves this role
- **Success**: `#6ABF4A` (Envy Green from extended palette, use sparingly)
- **Warning**: `#FF6A00` (Flame Orange, use sparingly)
- **Info**: `#3E8DDD` (Sapphire Blue, use sparingly)

### Interactive States
- **Button Default**: Signature Red `#E2232A`
- **Button Hover**: Deep Red `#64131E`
- **Button Pressed**: `#1E0013`
- **Focus Ring**: `#E2232A` at 2px solid
- **Link Default**: `#E2232A`
- **Link Visited**: `#64131E`
- **Disabled Text**: `#C4BEB6`
- **Disabled Background**: `#D9D8D6`

## 3. Typography Rules

### Font Families
- **Primary Display**: Montserrat Alternates Bold — used for logo and hero display moments
- **Primary Body**: Helvetica Neue — the core workhorse typeface across all communications
- **Online Fallback**: Lato, then Arial, then sans-serif
- **Chinese / CJK**: Han Yi Bold, Han Yi Medium, Han Yi Regular
- **Internal/Email**: Arial 10pt

```css
font-family: 'Helvetica Neue', 'Lato', Arial, sans-serif;
```

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|------|------|------|--------|-------------|----------------|
| Display Hero | Montserrat Alternates | 64px | 700 | 0.95 | -0.5px |
| Page Headline | Helvetica Neue | 48px | 300 | 0.95 | -0.3px |
| Section Heading | Helvetica Neue | 36px | 400 | 1.00 | -0.2px |
| Sub-heading | Helvetica Neue | 28px | 400 | 1.05 | -0.1px |
| Card Title | Helvetica Neue | 22px | 500 | 1.10 | normal |
| Large Body | Helvetica Neue | 18px | 300 | 1.55 | normal |
| Body | Helvetica Neue | 16px | 400 | 1.60 | normal |
| Body Emphasis | Helvetica Neue | 16px | 500 | 1.60 | normal |
| Small Body | Helvetica Neue | 14px | 400 | 1.50 | normal |
| Caption | Helvetica Neue | 13px | 400 | 1.40 | 0.1px |
| Caption Bold | Helvetica Neue | 13px | 500 | 1.40 | 0.1px |
| Label / Tag | Helvetica Neue | 12px | 500 | 1.33 | 0.5px |
| Micro | Helvetica Neue | 11px | 400 | 1.30 | 0.3px |
| Button | Helvetica Neue | 15px | 500 | 1.00 | 0.3px |
| Nav | Helvetica Neue | 14px | 400 | 1.00 | normal |

### Principles
- **95% leading at headline sizes**: Brand guide mandates headline leading at 95% of type size — tight, confident, authoritative
- **Light weight (300) for large display**: Use Ultralight/Light at 36px+ for an editorial, premium feel
- **Sentence case always**: Never all-caps for headlines in OneLenovo system — "Gotham Bold sentence case" is the stated rule
- **No decorative weights at small sizes**: Stick to 400 and 500 below 18px for legibility
- **Letter-spacing compressed at large sizes, neutral at body**: Negative tracking only at display, zero or slightly positive below 16px

## 4. Component Stylings

### Buttons

**Primary Red (Default CTA)**
- Background: `#E2232A`
- Text: `#FFFFFF`
- Font: Helvetica Neue 15px, weight 500, letter-spacing 0.3px
- Padding: 12px 28px
- Border Radius: 4px
- Hover: Background `#64131E`, transition 150ms ease
- Active: Background `#1E0013`
- Focus: 2px solid `#E2232A` outline, 2px offset

**Secondary Outlined**
- Background: transparent
- Text: `#E2232A`
- Border: 2px solid `#E2232A`
- Padding: 10px 26px
- Border Radius: 4px
- Hover: Background `#FAECEB`

**Ghost / Text Link**
- Background: transparent
- Text: `#E2232A`
- Underline on hover
- No border, no radius
- Arrow icon (→) as trailing element

**Dark / Inverse**
- Background: `#FFFFFF`
- Text: `#E2232A`
- Padding: 12px 28px
- Border Radius: 4px
- Used on dark/black backgrounds

**Disabled**
- Background: `#D9D8D6`
- Text: `#C4BEB6`
- Border: none
- Cursor: not-allowed

### Cards & Containers
- Background: `#FFFFFF`
- Border: 1px solid `#D9D8D6`
- Border Radius: 4px
- Shadow: `0 2px 8px rgba(0, 0, 0, 0.08)`
- Padding: 24px
- Hover: Border-color `#E2232A`, shadow `0 4px 16px rgba(226, 35, 42, 0.12)`

**Product Card**
- Image: full-width, 16:9 or 1:1 ratio, white/light bg
- Title: 22px, weight 500, `#1A1A1A`
- Spec line: 14px, weight 400, `#6F7170`
- Red CTA link at bottom
- Border top accent: 3px solid `#E2232A` on hover

### Input Fields
- Background: `#FFFFFF`
- Border: 1px solid `#C4BEB6`
- Border Radius: 4px
- Padding: 10px 14px
- Font: 16px, Helvetica Neue 400
- Placeholder: `#C4BEB6`
- Focus: Border 2px solid `#E2232A`, no shadow
- Error: Border 2px solid `#E2232A`, error text below in `#E2232A` 13px
- Disabled: Background `#D9D8D6`, text `#6F7170`

### Navigation
- Background: `#FFFFFF` (light) or `#000000` (dark hero variant)
- Height: 64px
- Border-bottom: 1px solid `#D9D8D6` (light)
- Logo: Lenovo wordmark in `#E2232A` and `#000000`, left-aligned
- Nav links: 14px, Helvetica Neue 400, `#1A1A1A`, hover color `#E2232A`
- Active link: `#E2232A` with 2px bottom border in `#E2232A`
- CTA button (rightmost): Primary Red button
- Mobile: Hamburger icon → full-screen drawer

### Tags & Labels
- Background: `#FAECEB`
- Text: `#E2232A`
- Padding: 4px 10px
- Border Radius: 2px
- Font: 12px, weight 500, letter-spacing 0.5px

### Red Rule Line
- A distinctive 3–4px horizontal rule in `#E2232A`
- Used to separate sections, accent headings, or bookend hero content
- Width: fixed (80px) under headings, or full-width between sections

## 5. Layout Principles

### Spacing System
- Base unit: **8px**
- Scale: 4, 8, 12, 16, 24, 32, 40, 48, 64, 80, 96, 128px
- Section vertical padding: 80px desktop, 48px tablet, 40px mobile

### Grid
- Max content width: **1200px** (1280px on wide viewports)
- Columns: 12-column grid with 24px gutters
- Side margins: 24px (mobile), 40px (tablet), auto (desktop, centered)
- No visible grid lines — whitespace creates separation

### Whitespace Philosophy
- **Red as punctuation, space as context**: Lenovo uses generous white space to let products breathe, with red lines and elements creating hierarchy
- **Product photography on white fields**: Never busy backgrounds behind product shots
- **One red moment per section**: Each content block has a single red focal element — CTA, headline accent, or rule line

### Border Radius Scale
- Sharp (0px): Data tables, technical grids
- Micro (2px): Tags, labels, badges
- Standard (4px): Buttons, cards, inputs, containers
- Medium (8px): Featured panels, image containers
- Large (16px): Full-bleed image modules
- Pill: Not used for buttons (Lenovo CTAs are rectangular, not pill-shaped)

## 6. Depth & Elevation

| Level | Shadow / Treatment | Use |
|-------|--------------------|-----|
| Flat (0) | No shadow | Navigation, body sections, tables |
| Lifted (1) | `0 2px 8px rgba(0,0,0,0.08)` | Cards, product tiles, dropdown menus |
| Floating (2) | `0 4px 16px rgba(0,0,0,0.12)` | Modal overlays, sticky headers on scroll |
| Brand Glow | `0 4px 16px rgba(226,35,42,0.15)` | Hovered product cards, focused red CTAs |
| Red Accent | 3px solid `#E2232A` top or left border | Active states, selected items, featured panels |

**Shadow Philosophy**: Lenovo's surfaces are largely flat. Depth is achieved through background-color contrast (white card on gray section) and the "brand glow" — a red-tinted shadow that only appears when the user interacts with a key element. This keeps the interface clean while making interactive moments feel charged and deliberate.

### Elevation via Color
- White on Off White: card-level separation
- Off White on White: section alternation
- Black section: hero/statement moments, inverts all text to white, CTAs to White or Red

## 7. Do's and Don'ts

### Do
- Use Signature Red (`#E2232A`) for ALL primary interactive elements — CTAs, links, active states
- Keep headlines at 95% line-height for that tight, confident brand voice
- Use Helvetica Neue Light (300) for large display text — premium editorial feel
- Alternate sections: white → off-white → black for rhythm and pacing
- Include exactly one red focal element per content section
- Use the L-pattern texture for branded backgrounds and event materials
- Write CTAs in sentence case — never ALL CAPS
- Add a 3–4px red rule line beneath section headings or above hero content
- Use Deep Purple (`#4D144A`) as a premium pairing with Red in special moments

### Don't
- Don't use Red for purely decorative purposes — it must signal action or brand
- Don't use more than one accent color per component (no Red + Purple together on same button)
- Don't use pill-shaped buttons — Lenovo CTAs are rectangular with 4px radius
- Don't use Helvetica Neue weight 700 or 900 — the scale stops at Medium (500)
- Don't use busy, patterned, or photographic backgrounds behind product images
- Don't apply wide letter-spacing to headlines — compress at large sizes
- Don't use all-caps for running text or headlines
- Don't use shadows heavier than `0 4px 16px rgba(0,0,0,0.12)` — the system is flat-first
- Don't put Red text on Red background
- Don't use the extended colors (Sapphire Blue, Envy Green, Flame Orange) without a semantic reason

## 8. Responsive Behavior

### Breakpoints
| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | <480px | Single column, 40px section padding |
| Mobile Large | 480–768px | Wider single column, 2-col product grid |
| Tablet | 768–1024px | 2–3 column grid, 48px section padding |
| Desktop Small | 1024–1280px | Full layout, 12-col grid |
| Desktop | 1280–1440px | Max content width 1200px, centered |
| Wide | >1440px | Locked at 1280px content width, open margins |

### Touch Targets
- Primary buttons: min 44px height
- Navigation links: 48px height touch area
- Cards: full-card tap target on mobile
- Form inputs: min 44px height

### Collapsing Strategy
- Hero headlines: 64px → 48px → 36px → 28px
- Navigation: horizontal links → hamburger → full-screen drawer
- Product grids: 4-col → 3-col → 2-col → 1-col
- Red rule lines: maintain width proportionally, never disappear
- Section padding reduces from 80px → 48px → 40px as viewport shrinks
- Cards stack vertically, never truncate text — use "show more" pattern instead

### Image Behavior
- Product images maintain 1:1 or 16:9 aspect ratio, never crop
- Hero images go full-bleed at all breakpoints
- White/neutral backgrounds on product shots persist at all sizes
- Lazy load all below-fold images

## 9. Agent Prompt Guide

### Quick Color Reference
- Primary CTA / Brand: Signature Red `#E2232A`
- Hover / Dark Red: `#64131E`
- Page Background: `#FFFFFF`
- Alt Section Background: `#D9D8D6`
- Dark / Hero Background: `#000000`
- Primary Text: `#1A1A1A`
- Secondary Text: `#6F7170`
- Disabled / Subtle: `#C4BEB6`
- Premium Accent: Deep Purple `#4D144A`
- Light Red Tint: `#FAECEB`
- Focus Ring: 2px solid `#E2232A`
- Card Shadow: `0 2px 8px rgba(0,0,0,0.08)`
- Brand Glow: `0 4px 16px rgba(226,35,42,0.15)`

### Example Component Prompts

- "Create a Lenovo hero section on a white background. Headline: 48px Helvetica Neue weight 300, line-height 0.95, letter-spacing -0.3px, color `#1A1A1A`. Subline: 18px weight 300, color `#6F7170`, line-height 1.55. Two CTAs: primary red button (`#E2232A`, white text, 12px 28px padding, 4px radius) and ghost text link with red `→`. Add a 4px horizontal rule in `#E2232A` beneath the headline."

- "Build a Lenovo product card: white background, 1px `#D9D8D6` border, 4px radius. Product image top half on white field (1:1 ratio). Title 22px Helvetica Neue weight 500 `#1A1A1A`. Spec text 14px weight 400 `#6F7170`. Bottom: red text link 'Learn more →' in `#E2232A`. On hover: border-color transitions to `#E2232A`, add `0 4px 16px rgba(226,35,42,0.12)` shadow."

- "Design Lenovo navigation: 64px height, white background, 1px bottom border `#D9D8D6`. Left: Lenovo wordmark. Center: nav links 14px Helvetica Neue 400 `#1A1A1A`, active link in `#E2232A` with 2px bottom underline. Right: primary red CTA button. On scroll >64px, add `0 2px 8px rgba(0,0,0,0.08)` shadow."

- "Create a Lenovo black hero section: background `#000000`, headline 48px Helvetica Neue weight 300 line-height 0.95 white. Subline 18px weight 300 `#C4BEB6`. CTA: white background, `#E2232A` text, 4px radius. Add L-pattern texture overlay at 5% opacity in white behind hero content."

- "Build a Lenovo data table: header row background `#1A1A1A`, header text white 13px weight 500 letter-spacing 0.5px. Body rows alternate white / `#D9D8D6`. Cell text 14px weight 400 `#1A1A1A`. Left column in weight 500. No border-radius. Add 3px left border in `#E2232A` on selected row."

### Iteration Guide
1. Every primary action gets Signature Red (`#E2232A`) — no other color takes that role
2. Headlines use Helvetica Neue Light (300) at large sizes — this is the premium signal
3. Line-height for headlines = 0.95 (95% of font size) — tight is right for Lenovo
4. Section rhythm: white → off-white → black, repeat; Red elements punctuate each
5. Cards use standard box shadow, add brand-glow on hover — subtle but charged
6. Deep Purple (`#4D144A`) is a premium reserve — use for special sections, not utility
7. One red moment per section: either a CTA, a rule line, an active state, or a headline accent
8. Buttons are rectangular (4px radius), never pill-shaped
9. Typography never all-caps; sentence case throughout
10. L-pattern textures can be used as background elements at very low opacity (3–8%) for brand richness without competing with content
