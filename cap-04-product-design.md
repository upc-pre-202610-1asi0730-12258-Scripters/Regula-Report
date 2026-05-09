# Chapter IV: Product Design

# 4.1. Style Guidelines

## 4.1.1. General Style Guidelines

Regula’s voice must reflect the product’s core values: security, efficiency, and trust. Every message, label, alert, or interface text must align with the following principles:

- **Reliable and professional:** Regula operates in high-responsibility environments (industrial safety, inventory control, leak detection). The language must convey technical solidity and institutional reliability, avoiding ambiguity.
- **Clear and direct:** Users are operators, supervisors, and distributors with high operational workloads. Messages must be concise, avoiding unnecessary technical jargon. Alerts and notifications must be immediately understandable.
- **Action-oriented:** Instructions, buttons, and CTAs should naturally encourage users to take action. Examples: "Register Entry", "View Alert", "Confirm Delivery", "Monitor Warehouse".
- **Approachable but not informal:** Regula communicates directly with the user, acknowledging the operational context of their work. The tone is neither cold corporate language nor excessively casual; it is empathetic and functional.
- **Focused on tangible benefits:** Messages highlight concrete outcomes: reduced losses, increased safety, real-time inventory control, and delivery traceability.

---

## Typography

Regula’s typography prioritizes functional readability on screen, especially in work environments where users need to quickly review dashboards, alerts, and records.

### Primary Typeface Family: Inter

Inter is a sans-serif typeface specifically designed for digital interfaces. It offers excellent readability at small and medium sizes, making it ideal for dashboards, forms, and operational text.

| Element | Typeface | Size | Weight | Primary Use |
|---|---|---|---|---|
| H1 – Page Title | Inter | 32px / 2rem | Bold 700 | Section names, main dashboard screen |
| H2 – Subtitle | Inter | 24px / 1.5rem | SemiBold 600 | Module subtitles, card headers |
| H3 – Heading | Inter | 20px / 1.25rem | SemiBold 600 | Widget, table, and form titles |
| Body – Main Text | Inter | 16px / 1rem | Regular 400 | Descriptive text, paragraphs, field labels |
| Small – Secondary | Inter | 14px / 0.875rem | Regular 400 | Metadata, timestamps, support text |
| Caption – Footer | Inter | 12px / 0.75rem | Medium 500 | Chart legends, tooltips, notes |
| Label – CTA | Inter | 14–16px | Bold 700 | Action buttons, status badges, alerts |

### Monospaced Typeface: JetBrains Mono

Specific use case: Gas cylinder codes, operation IDs, technical timestamps, and IoT sensor data where visual precision is required.

### Visual Hierarchy

- **Size contrast:** Titles should be at least 1.5× larger than body text to create a clear hierarchy.
- **Line height:** 1.5× font size for body text; 1.2× for titles and compact labels.
- **Line length:** Maximum 75 characters per line to ensure optimal readability on screen.

---

## Colors

| Color | Hex | Name | Usage |
|---|---|---|---|
| 🟠 | `#F26E22` | Active Orange | Primary CTA buttons, action icons, highlights |
| 🔶 | `#F25922` | Alert Orange | Leak alerts, critical states, risk indicators |
| 🩶 | `#A5B1BF` | Steel Gray | Borders, dividers, secondary text, inactive icons |
| ⬜ | `#F8F8FB` | Ice White | General background, card backgrounds, base surfaces |
| ⬜ | `#FFFFFF` | Pure White | Text on dark backgrounds, icons on navy/orange |
| ⬛ | `#111111` | Soft Black | Main text with high readability on light backgrounds |
| 🔘 | `#555F6E` | Medium Gray | Body text, labels, metadata |
| 🔲 | `#E8ECF0` | Light Gray | Alternate table row backgrounds, subtle dividers |

### Color Descriptions

- **Deep Navy Blue (`#172D40`):** Primary brand color. Conveys trust, control, and technical seriousness. Used in headers, sidebars, main titles, and navigation elements. It is the anchor color of Regula’s identity.
- **Active Orange (`#F26E22`):** Primary accent color representing energy, positive urgency, and operational visibility. Ideal for primary CTA buttons, highlighted icons, and first-level interactive elements.
- **Alert Orange (`#F25922`):** A more intense variation of orange. Used for high-urgency alerts, moderate-to-high risk indicators, and active critical states such as leak detection or "in transit" status.
- **Steel Gray (`#A5B1BF`):** Neutral cool color. Complements navy blue in secondary elements: borders, dividers, support text, inactive icons, and neutral card backgrounds.
- **Ice White (`#F8F8FB`):** Main interface background. Provides visual cleanliness, soft contrast, and reduces eye strain during long work sessions.

---

## Spacing

| Value | Rem | Usage |
|---|---|---|
| 4px | 0.25rem | Minimal spacing between related elements (icons + text, label + input) |
| 8px | 0.5rem | Internal padding for badges, chips, and compact labels |
| 12px | 0.75rem | Spacing between lines of text in cards and lists |
| 16px | 1rem | Standard padding for cards, form fields, and base containers |
| 24px | 1.5rem | Separation between sections within a module or large card |
| 32px | 2rem | Space between cards, dashboard widgets, and main modules |
| 48–64px | 3–4rem | Margin between full-page sections or differentiated content blocks |

---

## Layout

### Layout Principles

- **12-column grid:** Responsive layout based on a 12-column grid with 16–24px gutters. Mobile: 4 columns; tablet: 8; desktop: 12.
- **Maximum content width:** 1280px for full-page containers. Centered with automatic side margins.
- **Fixed sidebar:** Side navigation with a width of 240–260px. Collapsible to 64px in compact mode for greater workspace area.
- **Cards and panels:** Border radius of 10–12px. Soft shadow: `box-shadow: 0 2px 8px rgba(23,45,64, 0.08)`. Avoid harsh borders on light backgrounds.
- **Data tables:** Minimum row height of 48px. Alternate rows between `#FFFFFF` and `#F8F8FB`. Table headers use `#172D40` with white text.
- **Forms:** Labels positioned above fields (not inline). Fields use `border: 1px solid #A5B1BF`. Focus state: orange border (`#F26E22`) + subtle shadow.
- **Information hierarchy:** Follow the pattern: section title → subtitle → content → secondary actions. Never mix hierarchy levels within the same area.

---

## Components

### Buttons

- **Primary (Main CTA):** Background `#F26E22`, white text, `border-radius: 8px`, padding `12×24px`. Hover: `#F25922`. Used for primary actions such as "Register Entry", "Save", "Confirm".
- **Secondary:** Border `1.5px #172D40`, text `#172D40`, transparent background. Hover: `#172D40` background + white text. Used for support actions.
- **Destructive / Alert:** Background `#EF4444`, white text. Exclusively for deleting, canceling deliveries, or confirming critical alerts.
- **Disabled:** Background `#E8ECF0`, text `#A5B1BF`. Non-clickable, `cursor: not-allowed`.

### Badges and States

| State | Background | Text | Usage |
|---|---|---|---|
| Operational / Normal | `#DCFCE7` | `#15803D` | Cylinders in good condition, warehouse without alerts |
| In Transit / Active | `#FEF3C7` | `#B45309` | Deliveries in progress, active sensors |
| Alert / Warning | `#F25922` | White | Gas detections, delays, or anomalies |
| Error / Critical | `#FEE2E2` | `#DC2626` | Confirmed leaks, connection losses, discarded cylinders |

### Alerts and Notifications

- **Style:** Banner at the top of the screen or side notification panel. Should not interrupt workflow (no modals for informational alerts).
- **High urgency (leak detected):** Red or intense orange banner with warning icon + short text + "View Details" button. Optional alert sound in desktop version.
- **Medium urgency (low inventory):** Informative yellow-orange banner. Can be manually dismissed.
- **Low urgency (reminder):** Toast notification in the bottom-right corner. Automatically disappears after 5 seconds.

---

## Accessibility

- **Text contrast:** Minimum 4.5:1 for normal text; 3:1 for large text (18px+ bold). Orange (`#F26E22`) on white meets this standard.
- **UI component contrast:** Minimum 3:1 for field borders, functional icons, and interactive elements.
- **Not color alone:** Never communicate information using only color. Always accompany with icons, text, or patterns (especially for alerts and error states).
- **Minimum touch target:** 44×44px for interactive elements on touch devices (field tablets, mobile phones).
- **Visible focus:** Clearly visible focus state with orange outline or thick border `#F26E22` of 2–3px. Never remove the native outline without replacement.
- **Alternative text:** All functional icons and dashboard graphics must include descriptive `aria-label` attributes.

# 4.1.2. Web Style Guidelines

## Supported Devices

| Device | Breakpoint | Columns | Behavior |
|---|---|---|---|
| Mobile | < 640px | 4 columns | Hamburger navigation, stacked layout, full-width cards |
| Tablet | 640–1023px | 8 columns | Collapsible sidebar, 2-column cards, visible navigation |
| Desktop | 1024–1279px | 12 columns | Full layout, fixed sidebar, 3-column cards |
| Wide | ≥ 1280px | 12 columns | Maximum centered width of 1280px, automatic side margins |

- **Mobile-first:** Design first for mobile and progressively add visual complexity as viewport size increases.
- **Adaptive navigation:** Hamburger menu on mobile (< 640px); full horizontal navigation on tablet and desktop.
- **Responsive images:** Use `srcset` and relative sizing. Never fix widths in absolute pixels for content images.
- **Fluid typography:** Font sizes scale with viewport using `clamp()` or responsive utility classes.
- **Touch targets:** Every interactive element must have a minimum touch area of 44×44px on mobile.
- **Tablet dashboard:** Real-time gas metrics dashboard is hidden or simplified on mobile; fully displayed on tablet and desktop.

---

## User Communication

- **Reliable and professional:** Qlic operates in contexts where data is critical (leaks, pressure, temperature). The language conveys technical solidity without sounding cold or distant. Users trust the data because the system communicates with authority.
- **Approachable and empathetic:** The platform speaks directly to the user. It acknowledges real user needs —preventing waste, avoiding damage— and communicates accordingly. Avoid unnecessary technical jargon.
- **Clear and direct:** Avoid ambiguity. Each message communicates one idea. Alerts must be immediately understandable: users know what happened and what to do next.
- **Focused on tangible benefits:** Texts emphasize concrete results for households (preventing leaks) and businesses (audits, compliance, cost reduction).
- **No technical jargon in UI:** Terms such as volume or bar may appear in metrics, but they should include context (e.g., green/yellow/red status indicators) so non-technical users can also understand them.

---

## Typography

| Element | Typeface | Size | Weight | Line-height | Usage |
|---|---|---|---|---|---|
| Display / Hero | Poppins | 48–56px | 700 Bold | 1.1 | Main title in hero section |
| H1 Page | Poppins | 36–40px | 700 Bold | 1.2 | Main section headers |
| H2 Section | Poppins | 28–32px | 600 SemiBold | 1.3 | Section and module subtitles |
| H3 Card | Poppins | 20–24px | 600 SemiBold | 1.4 | Card and widget titles |
| Body Large | Roboto | 18px | 400 Regular | 1.6 | Hero and About Us descriptions |
| Body Base | Roboto | 16px | 400 Regular | 1.6 | General paragraphs and content |
| Body Small | Roboto | 14px | 400 Regular | 1.5 | Metadata, labels, card footers |
| Caption | Roboto | 12px | 400 Regular | 1.4 | Legends, tooltips, legal notes |
| Button / Label | Poppins | 14–16px | 600 SemiBold | 1.0 | CTA buttons, badges, navigation |
| Price / Metric | Poppins | 32–40px | 700 Bold | 1.1 | Pricing plans, dashboard metrics |

---

## Colors

### Color Descriptions

- **Primary Blue (`#0C4AFD`):** Primary brand color. Conveys technology, trust, and precision. Present in the header, navigation, general CTA buttons, action icons, and brand identity elements.
- **Dark Blue (`#0A1F6E`):** Used for high-contrast text on light backgrounds, main titles, and highest hierarchy brand elements. Provides seriousness and authority.
- **Medium Blue (`#3B82F6`):** Accessible blue variation for most interactive CTA buttons: "Get Started", "Choose Plan", hover states, and active links.
- **Green (`#22C55E`):** Accent color for success and specific actions. Used exclusively for the "Send" button in the contact form, the "Real-Time Water Monitoring" badge, and normal operational status indicators.
- **Black (`#0F0F0F`):** Used for section titles, high-legibility main text, and impactful headings. Ensures AAA contrast on light backgrounds.
- **Dark Gray (`#374151`):** Used for general body text, paragraphs, card descriptions, and most textual content throughout the platform.
- **Medium Gray (`#6B7280`):** Used for secondary text, metadata, timestamps, placeholders, and lower hierarchy content.
- **Light Gray (`#F3F4F6`):** Used for alternate section backgrounds, even table rows, neutral card backgrounds, and subtle visual dividers.
- **White (`#FFFFFF`):** Main platform background, card surfaces, modals, and panels. Also used for text on dark backgrounds (blue headers, primary buttons).

### Color Palette

| Color | Hex | Name | Role | Primary Usage |
|---|---|---|---|---|
| 🔵 | `#0C4AFD` | Primary Blue | Primary | Header, navigation, branding elements, active badge |
| 🟦 | `#0A1F6E` | Dark Blue | Secondary | Section titles, high hierarchy text |
| 💙 | `#3B82F6` | Medium Blue | General CTA | Buttons: Get Started, Choose Plan, interactive CTAs |
| 🟢 | `#22C55E` | Green | Accent | Send button (form), Real-Time badge, normal status |
| ⬛ | `#0F0F0F` | Black | Text | H1/H2 titles, section headers, hero text |
| 🔘 | `#374151` | Dark Gray | Text | General body text, paragraphs, descriptions |
| 🔲 | `#6B7280` | Medium Gray | Secondary | Support text, metadata, placeholders, timestamps |
| ⬜ | `#F3F4F6` | Light Gray | Background | Alternate sections, table rows, neutral backgrounds |
| ⬜ | `#F9FAFB` | Soft White | Surface | Card backgrounds, inputs, content panels |
| ⬜ | `#FFFFFF` | Pure White | Base | Main site background, modals, text on dark backgrounds |
| 🔳 | `#E5E7EB` | Border Gray | Neutral | Card borders, inputs, dividers, separators |
| 🔷 | `#EFF6FF` | Very Light Blue | Accent Background | Blue badge backgrounds, informational highlights |
| 🟩 | `#F0FDF4` | Very Light Green | Accent Background | Real-time badge background |

### Color Usage Rules

- **One green button per page:** Green (`#22C55E`) is exclusive to the "Send" button in the contact form and the real-time status badge. Do not use green for other buttons or CTAs to preserve its unique semantic meaning.
- **Blue as the dominant color:** Blue in its three variations (primary, dark, medium) is the anchor color of the brand. It must always be present in the header and navigation throughout the platform.
- **Alternating backgrounds:** Alternate between white (`#FFFFFF`) and very light gray (`#F3F4F6`) section backgrounds across the landing page to create visual rhythm without using large brand-colored backgrounds.
- **Minimum WCAG AA contrast:** All text on colored backgrounds must meet a minimum contrast ratio of 4.5:1. White text on primary blue (`#0C4AFD`) meets this standard.
- **No colors outside the palette:** No UI element should introduce colors not defined in this guide without approval from the design team.

---

## Spacing

| Token | Value px | Value rem | Typical Usage |
|---|---|---|---|
| space-1 | 4px | 0.25rem | Minimal separation between icon and inline text |
| space-2 | 8px | 0.5rem | Internal padding for badges, chips, and tags |
| space-3 | 12px | 0.75rem | Gap between list elements, icons, and nav labels |
| space-4 | 16px | 1rem | Standard padding for cards, form fields, containers |
| space-6 | 24px | 1.5rem | Gap between cards within a section, small section padding |
| space-8 | 32px | 2rem | Separation between subsections, container side padding |
| space-12 | 48px | 3rem | Margin between major landing page sections |
| space-16 | 64px | 4rem | Top and bottom padding for hero and impact sections |
| space-24 | 96px | 6rem | Maximum separation between differentiated content blocks |

---

## Buttons

- **Padding:** `12px 24px` (medium) · `10px 20px` (small) · `16px 32px` (large)
- **Border-radius:** `8px` for all buttons. Consistency across the entire platform.
- **Font:** Poppins SemiBold 600, 14–16px, `letter-spacing: 0.01em`
- **Hover state:** Reduce opacity to 90% or lighten the base color by 10%. Transition `150ms ease`.
- **Focus state:** `3px` outline with `2px` offset using the button color at 40% opacity. Never remove focus without replacement.
- **Loading state:** Spinner inside the button, text changes to "Loading...", button disabled.






