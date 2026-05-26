# 1% Professional Website Design Options

Use this when choosing color, shadow, radius, spacing, typography, surfaces, buttons, cards, tables, charts, and overall visual direction for HTML/CSS/JS/SQL sites, ERP, CRM, SaaS, admin, and analytics apps.

## Golden Rules

- Pick 1 primary accent, 1 optional secondary accent, neutral surfaces, and semantic status colors.
- Keep backgrounds calm; put color on actions, status, charts, and key highlights.
- Use one shadow scale, one radius scale, one spacing scale, one icon style.
- Prefer borders and spacing over heavy shadows for professional business tools.
- Use high contrast: body text `4.5:1`, UI borders/icons `3:1`.
- Never use color alone for meaning; add label/icon/text.
- Avoid one-note palettes, excessive purple gradients, beige-only pages, decoration blobs, and random glass effects.
- Use real content density. ERP/CRM/admin should be quiet, scannable, and efficient.

## Option 1: Enterprise Clean

Best for ERP, CRM, admin, analytics, healthcare, logistics, internal tools.

```css
:root {
  --bg: #f8fafc;
  --surface: #ffffff;
  --surface-2: #f1f5f9;
  --text: #0f172a;
  --muted: #64748b;
  --border: #dbe3ef;
  --primary: #2563eb;
  --primary-strong: #1d4ed8;
  --secondary: #0f766e;
  --success: #15803d;
  --warning: #b45309;
  --danger: #b91c1c;
}
```

Visual rules:
- Header/sidebar: white surface, subtle bottom/right border.
- Buttons: solid primary for main action, outline/ghost for secondary.
- Cards: white with border, very soft shadow only for raised panels.
- Tables: white rows, slate text, light blue selected row.

## Option 2: Modern SaaS

Best for subscriptions, dashboards, productivity tools, AI tools.

```css
:root {
  --bg: #f6f8fb;
  --surface: #ffffff;
  --surface-2: #eef2f7;
  --text: #111827;
  --muted: #6b7280;
  --border: #d8dee8;
  --primary: #4f46e5;
  --primary-strong: #3730a3;
  --secondary: #0891b2;
  --success: #16a34a;
  --warning: #d97706;
  --danger: #dc2626;
}
```

Visual rules:
- Use color mostly on CTAs, active nav, progress, and charts.
- Pair primary with cyan sparingly; do not turn whole page purple.
- Rounded `8px` max for cards; `6px` for inputs/buttons.

## Option 3: Finance Trust

Best for fintech, accounting, invoices, payments, B2B sales.

```css
:root {
  --bg: #f7f9fc;
  --surface: #ffffff;
  --surface-2: #edf2f7;
  --text: #0b1220;
  --muted: #526173;
  --border: #d6dee9;
  --primary: #0f5e9c;
  --primary-strong: #0b4473;
  --secondary: #0f766e;
  --success: #047857;
  --warning: #b7791f;
  --danger: #b42318;
}
```

Visual rules:
- Use compact spacing, sharp hierarchy, clear totals, tabular numbers.
- Avoid playful shadows and loud gradients.
- Money fields right-aligned with stable decimal formatting.

## Option 4: Premium Editorial

Best for portfolios, agencies, luxury, premium services, brand sites.

```css
:root {
  --bg: #fbfaf8;
  --surface: #ffffff;
  --surface-2: #f0ede8;
  --text: #111111;
  --muted: #66615b;
  --border: #d8d2c8;
  --primary: #111111;
  --secondary: #b88a2e;
  --success: #2f7d4f;
  --warning: #a16207;
  --danger: #b91c1c;
}
```

Visual rules:
- Use whitespace, typography, and image quality as the design.
- Buttons can be black/white with thin borders.
- Shadows almost none; use hairline borders and strong type.
- Not ideal for dense ERP/CRM screens unless heavily restrained.

## Option 5: Healthcare Calm

Best for clinics, hospital systems, appointment tools, patient portals.

```css
:root {
  --bg: #f5fbfb;
  --surface: #ffffff;
  --surface-2: #e8f4f4;
  --text: #102326;
  --muted: #5f7478;
  --border: #cfe0e2;
  --primary: #0f766e;
  --primary-strong: #115e59;
  --secondary: #0284c7;
  --success: #15803d;
  --warning: #b45309;
  --danger: #be123c;
}
```

Visual rules:
- Keep contrast strong despite calm colors.
- Use clear status labels for urgent/waiting/completed/cancelled.
- Avoid pale gray text on pale blue/green backgrounds.

## Option 6: Operations Dark

Best for monitoring, analytics walls, technical dashboards, support consoles.

```css
:root {
  --bg: #0b1020;
  --surface: #111827;
  --surface-2: #172033;
  --text: #f8fafc;
  --muted: #a8b3c7;
  --border: #263348;
  --primary: #38bdf8;
  --primary-strong: #0ea5e9;
  --secondary: #22c55e;
  --success: #4ade80;
  --warning: #facc15;
  --danger: #fb7185;
}
```

Visual rules:
- Use dark mode only when it improves monitoring or brand fit.
- Borders must be visible; muted text still needs contrast.
- Charts need brighter but limited colors; avoid neon overload.

## Option 7: Marketplace Warm

Best for directories, logistics listings, service marketplaces, community commerce.

```css
:root {
  --bg: #f9faf6;
  --surface: #ffffff;
  --surface-2: #eef2e8;
  --text: #1f2933;
  --muted: #667085;
  --border: #d8dfcf;
  --primary: #256f5b;
  --primary-strong: #1f5c4c;
  --secondary: #c2410c;
  --success: #15803d;
  --warning: #b45309;
  --danger: #b91c1c;
}
```

Visual rules:
- Use warm accent only for highlights, tags, and secondary actions.
- Good for cards/listings, but keep filter UI clean and businesslike.

## Option 8: High-Contrast Minimal

Best for documentation, developer tools, legal, compliance, simple admin.

```css
:root {
  --bg: #ffffff;
  --surface: #ffffff;
  --surface-2: #f4f4f5;
  --text: #09090b;
  --muted: #52525b;
  --border: #d4d4d8;
  --primary: #18181b;
  --secondary: #2563eb;
  --success: #166534;
  --warning: #a16207;
  --danger: #991b1b;
}
```

Visual rules:
- Strong text, thin borders, minimal shadow.
- Excellent for docs/admin where clarity beats decoration.

## Shadow Scale

Use one scale only:

```css
:root {
  --shadow-xs: 0 1px 2px rgba(15, 23, 42, 0.06);
  --shadow-sm: 0 2px 6px rgba(15, 23, 42, 0.08);
  --shadow-md: 0 8px 24px rgba(15, 23, 42, 0.10);
  --shadow-lg: 0 18px 48px rgba(15, 23, 42, 0.14);
}
```

Usage:
- Inputs, tables, nav: border only, no shadow.
- Cards: border plus `--shadow-xs` only when raised.
- Dropdowns/popovers: `--shadow-md`.
- Modals: `--shadow-lg` plus scrim.
- ERP/CRM/admin: prefer borders over shadows.
- Landing pages: one hero/media shadow allowed; do not shadow every card.

Dark mode shadows:

```css
:root {
  --shadow-xs: 0 1px 2px rgba(0, 0, 0, 0.25);
  --shadow-sm: 0 4px 12px rgba(0, 0, 0, 0.30);
  --shadow-md: 0 12px 32px rgba(0, 0, 0, 0.38);
  --shadow-lg: 0 24px 64px rgba(0, 0, 0, 0.45);
}
```

In dark mode, use borders and lighter surfaces more than shadows.

## Radius Scale

```css
:root {
  --radius-xs: 3px;
  --radius-sm: 4px;
  --radius-md: 6px;
  --radius-lg: 8px;
  --radius-pill: 999px;
}
```

Usage:
- Inputs/buttons: `6px`.
- Cards/panels: `6-8px`.
- Badges/chips: pill.
- Tables: outer wrapper `8px`, rows square inside.
- Modals: `8px`.
- Avoid `16-32px` rounded business UI unless brand is playful.

## Border And Surface Rules

- Page bg: very light neutral, not pure white when many panels exist.
- Primary surface: white or dark panel.
- Secondary surface: subtle tinted neutral for filters/toolbars.
- Border: visible enough to separate panels, not black.
- Active item: tinted background plus colored left bar/dot/bold text.
- Disabled: lower opacity plus disabled attribute, not just pale color.
- Selected row: subtle primary tint, checkbox selected, count visible.

## Button Rules

- One primary action per screen.
- Primary: solid primary color, white text, strong hover.
- Secondary: white/transparent with border.
- Ghost: nav/tool actions only.
- Danger: red text or red outline by default; solid red only for final destructive confirmation.
- Icon-only buttons need `aria-label`, tooltip, `44x44px` hit area.
- Loading button keeps width stable and shows spinner/text.

## Typography Options

System safest:

```css
font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
```

Premium editorial:

```css
font-family: "Source Serif 4", Georgia, serif;
```

Developer/data:

```css
font-family: ui-sans-serif, system-ui, sans-serif;
font-variant-numeric: tabular-nums;
```

Scale:
- label: `12px`, medium, line `16px`
- small/body secondary: `14px`, line `20px`
- body: `16px`, line `24px`
- h3: `20px`, line `28px`
- h2: `28-32px`, line `36-40px`
- h1: `40-56px` landing, `24-32px` app pages

## Gradients

Use gradients sparingly:

- Good: CTA hover, chart area fade, subtle hero image overlay, status heatmap.
- Bad: full page gradient background for ERP/CRM/admin.
- Use 2 colors max plus alpha; no rainbow UI.
- Keep text on solid or dark overlay, not busy gradient.

Professional examples:

```css
background: linear-gradient(135deg, #2563eb, #0891b2);
background: linear-gradient(180deg, rgba(15,23,42,0.72), rgba(15,23,42,0.18));
```

## Chart Colors

Use accessible, distinct series:

```css
--chart-1: #2563eb;
--chart-2: #0f766e;
--chart-3: #f59e0b;
--chart-4: #dc2626;
--chart-5: #7c3aed;
--chart-6: #475569;
```

Rules:
- Trend: line chart, 1-3 series.
- Comparison: bar chart.
- Composition: stacked bar or donut only for <=5 categories.
- KPI: value, label, delta, period, tiny trend if useful.
- Add labels/tooltips/table fallback.
- Do not use red/green as only distinction.

## ERP/CRM/Admin Look

- Palette: Enterprise Clean, Finance Trust, or High-Contrast Minimal.
- Layout: sidebar, top bar, filters, table, detail drawer.
- Surfaces: white panels, light neutral bg, clear borders.
- Shadows: almost none; dropdown/modal only.
- Density: compact but not cramped. Row height `44-52px`.
- Status: chip text plus color.
- Charts: restrained; analytics should be readable, not decorative.

## Landing/Marketing Look

- Palette: Modern SaaS, Premium Editorial, Marketplace Warm, or brand-specific.
- Header: airy, logo left, nav center/right, CTA right.
- Hero: strong type, real product/place/person visual, CTA, proof.
- Shadows: one hero/media shadow plus soft cards.
- Sections: generous vertical spacing, visible next section, no card-in-card.
- Footer: required for trust, legal, contact, social.

## Missed-Item Checklist

- Color tokens for light and dark mode.
- Hover/focus/pressed/disabled/loading states.
- Status colors for success/warning/danger/info.
- Border, radius, and shadow scales.
- Table density, selected row, sticky header.
- Form labels, helper text, errors, required state.
- Empty/loading/error/no-permission/no-results states.
- Chart palette, legends, labels, table fallback.
- Mobile card alternative for tables.
- Print/export styling for reports.
- Contrast checked for every text/surface pair.
