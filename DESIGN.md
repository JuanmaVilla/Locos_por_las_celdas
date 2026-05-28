# Efficient Ledger — Design System

## Brand & Style

**Modern Corporate** aesthetic for educational/productivity sector. Evokes reliability, efficiency, professional mastery. Clean structure with ample white space. "Tactile-lite" elements (soft shadows, crisp flat iconography). Emojis add human/mentor tone. Mentor feel, not a manual.

---

## Colors

### Surface Scale
| Token | Value |
|---|---|
| `background` / `surface` / `surface-bright` | `#fcf9f8` |
| `surface-container-lowest` | `#ffffff` |
| `surface-container-low` | `#f6f3f2` |
| `surface-container` | `#f0eded` |
| `surface-container-high` | `#eae7e7` |
| `surface-container-highest` | `#e4e2e1` |
| `surface-dim` | `#dcd9d9` |
| `surface-variant` | `#e4e2e1` |
| `inverse-surface` | `#303030` |

### On-Surface
| Token | Value |
|---|---|
| `on-surface` | `#1b1c1c` |
| `on-surface-variant` | `#3f4941` |
| `on-background` | `#1b1c1c` |
| `inverse-on-surface` | `#f3f0f0` |

### Outlines
| Token | Value |
|---|---|
| `outline` | `#6f7a70` |
| `outline-variant` | `#bfc9be` |
| `surface-tint` | `#176c40` |

### Primary — Excel Green
| Token | Value |
|---|---|
| `primary` | `#005931` |
| `on-primary` | `#ffffff` |
| `primary-container` | `#217346` |
| `on-primary-container` | `#a4f5bd` |
| `inverse-primary` | `#88d8a1` |
| `primary-fixed` | `#a3f4bc` |
| `primary-fixed-dim` | `#88d8a1` |
| `on-primary-fixed` | `#00210f` |
| `on-primary-fixed-variant` | `#00522d` |

> Primary = high-impact actions, headlines, active states.

### Secondary — Soft Green Tint
| Token | Value |
|---|---|
| `secondary` | `#556158` |
| `on-secondary` | `#ffffff` |
| `secondary-container` | `#d9e6da` |
| `on-secondary-container` | `#5b675e` |
| `secondary-fixed` | `#d9e6da` |
| `secondary-fixed-dim` | `#bdcabe` |
| `on-secondary-fixed` | `#131e17` |
| `on-secondary-fixed-variant` | `#3e4a41` |

> Secondary = section backgrounds, highlights, visual fatigue reduction.

### Tertiary — Light Gray
| Token | Value |
|---|---|
| `tertiary` | `#4c4d4e` |
| `on-tertiary` | `#ffffff` |
| `tertiary-container` | `#646565` |
| `on-tertiary-container` | `#e3e3e3` |
| `tertiary-fixed` | `#e2e2e2` |
| `tertiary-fixed-dim` | `#c6c6c7` |
| `on-tertiary-fixed` | `#1a1c1c` |
| `on-tertiary-fixed-variant` | `#454747` |

> Tertiary = alternating section backgrounds, subtle UI containers.

### Error
| Token | Value |
|---|---|
| `error` | `#ba1a1a` |
| `on-error` | `#ffffff` |
| `error-container` | `#ffdad6` |
| `on-error-container` | `#93000a` |

### Section Alternation Pattern
`White (#ffffff)` → `Light Green (#d9e6da)` → `White` → `Very Light Gray (#e2e2e2)`

---

## Typography

Font: **Inter** exclusively. No exceptions.

| Token | Family | Size | Weight | Line Height | Letter Spacing |
|---|---|---|---|---|---|
| `display-lg` | Inter | 48px | 800 | 1.1 | -0.02em |
| `display-lg-mobile` | Inter | 32px | 800 | 1.2 | — |
| `headline-md` | Inter | 32px | 700 | 1.3 | — |
| `headline-sm` | Inter | 24px | 700 | 1.4 | — |
| `body-lg` | Inter | 18px | 400 | 1.6 | — |
| `body-md` | Inter | 16px | 400 | 1.5 | — |
| `label-bold` | Inter | 14px | 700 | 1 | — |

Headlines: bold/extra-bold, tight letter-spacing, commands attention.  
Body: regular weight, generous line-height for long-form reading.  
Mobile: display sizes scale down for comfortable rhythm.

---

## Layout & Spacing

| Token | Value |
|---|---|
| `base` | 8px |
| `section-padding-desktop` | 80px |
| `section-padding-mobile` | 48px |
| `gutter` | 24px |
| `stack-sm` | 12px |
| `stack-md` | 24px |
| `container-max-width` | 1140px |

Desktop: Fixed grid, content centered in 1140px container.  
Mobile: Fluid single-column, 20px side margins.  
All spacing derived from 8px base unit.

---

## Border Radius

| Token | Value |
|---|---|
| `rounded-sm` | 0.25rem (4px) |
| `rounded` / `rounded-DEFAULT` | 0.5rem (8px) |
| `rounded-md` | 0.75rem (12px) |
| `rounded-lg` | 1rem (16px) |
| `rounded-xl` | 1.5rem (24px) |
| `rounded-full` | 9999px |

Default radius = **8px**. Softens Excel grid rigidity, keeps professional look.  
- Cards & Accordions: 8px  
- Buttons: 8px (no pill shapes)  
- Checkboxes: 4px

---

## Elevation & Depth

**Flat-plus** approach. Depth via color-blocking, not heavy shadows.

- **Default surfaces:** flat, no shadow
- **Interactive elements (cards, buttons on hover):** `box-shadow: 0px 10px 30px rgba(0, 0, 0, 0.05)`
- **Containers (tables, inputs):** 1px border in slightly darker background shade (e.g., `#D0E8D2` on green sections)

---

## Components

### Buttons — Primary
- Background: `#217346` (`primary-container`)
- Text: `#ffffff`, Inter bold
- Min-height: 56px
- Padding: 32px horizontal
- Border-radius: 8px
- Hover: soft shadow (`0px 10px 30px rgba(0,0,0,0.05)`) + slight scale lift
- No pill shapes

### Feature Cards (Modules / Bonuses)
- Background: `#ffffff`
- Border: 1px `#e4e2e1` (`outline-variant` range)
- Border-radius: 8px
- Emoji or flat icon top-left for category
- Hover: shadow `0px 10px 30px rgba(0,0,0,0.05)`

### Accordions (FAQ)
- Borderless style
- Alternating gray/white row backgrounds
- Chevron icon, rotates 180° on expand
- Question text: `body-lg` bold
- Answer text: `body-md` regular

### Comparison Tables (Before vs. After)
- "After" column: light green background (`#d9e6da`)
- "Before" column: light gray background (`#e2e2e2`)
- Positive indicators: ✅ green checkmark emoji
- Negative indicators: ❌ muted gray x emoji
- 1px border `#D0E8D2` to define container

### Input Fields
- Background: `#ffffff`
- Border: 1px `outline-variant` (`#bfc9be`)
- Border-radius: 8px
- Focus state: border transitions to `#217346` (Excel Green) + subtle outer glow
- Label: `label-bold`
