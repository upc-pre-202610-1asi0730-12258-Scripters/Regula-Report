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



## 4.2. Information Architecture

Regula’s Information Architecture has been designed with the goal of organizing content in a clear, intuitive, and efficient manner, allowing both gas companies and distributors to quickly access the system’s key functionalities. Since users have a low level of digitalization and are accustomed to manual processes, the structure prioritizes simplicity, speed, and visibility of critical information.

## 4.2.1. Organization Systems

* **Hierarchical:**
  Organized from the most important elements (**operational safety, gas leak detection, and initial CTA**) to the most detailed ones (**subscription plans, FAQ, and contact**).

* **Sequential:**
  Follows a natural flow:
  **What it is → Who we are → Solutions → Features → Pricing → Contact**.

* **By audience:**
  Clear differentiation between:

    * **Gas bottling companies:** warehouse monitoring and cylinder control.
    * **Distributors:** daily inventory management, deliveries, and collections.

* **By functionality:**
  Grouping of technical capabilities:

    * Gas leak detection with IoT sensors
    * Gas cylinder entry and exit registration
    * Real-time delivery tracking

---

### Site Structure

| Topic | Definition |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| **Home** | General overview of the platform, highlighting leak monitoring, inventory control, and real-time tracking, together with the main CTA. |
| **Solutions** | Differentiates segments: gas bottling companies (warehouses and alerts) and distributors (inventory, deliveries, and collections). |
| **Features** | Technical capabilities: leak detection, gas cylinder registration, and real-time tracking. |
| **Pricing** | Plans (Basic, Standard, Premium) according to operational needs. |
| **Testimonials** | Opinions from real users to build trust. |
| **Contact** | Direct channel for inquiries and contact with the team. |
| **FAQ** | Frequently asked questions about compatibility, IoT connectivity, and alerts. |

---

## 4.2.2. Labeling Systems

Regula’s labeling system prioritizes **simplicity, clarity, and familiarity**, considering users with low levels of digitalization.

### Labeling Principles

* **Use of few words (max. 2–3):**
  Facilitates quick reading and reduces cognitive load.

* **Natural user language:**
  Example: *“Cylinder Exit”* instead of *“Inventory Dispatch”*.

* **Terminology consistency:**
  Consistent use of the term *“cylinder”* throughout the system.

* **Focus on action + object:**
  Allows users to quickly understand each option.

---

### Main Labels

* Dashboard
* Alerts
* Entries
* Exits
* Stock
* Deliveries
* Sales
* Debts
* History

These represent key functions: **inventory, safety, distribution, and operations**.

---

### Secondary Labels

* Register Entry
* Register Exit
* View Details
* Mark as Resolved
* Assign Delivery
* Update Status
* Filter
* Search

Use of **direct verbs** for intuitive interaction.

---

### States and Alerts

* Normal
* Alert
* Leak Detected
* Pending
* Resolved

Allow users to quickly identify risks and tasks.

---

### Label Association

* **Entries / Exits → Stock → History**
  (inventory control)

* **Deliveries → Sales → Debts**
  (commercial flow)

* **Alerts → Dashboard**
  (monitoring and decision-making)

---

### Cross-Platform Consistency

* Same labels on web and mobile
* Immediate recognition
* Continuity of use

---

### Justification

* Users use simple operational language
* Low familiarity with complex systems
* Need for speed in tasks

---

## 4.2.3. SEO Tags and Meta Tags

* **Title:**
  *Regula – Smart Gas Cylinder Monitoring and Management System*

* **Description:**
  Optimize the management of gas cylinders with IoT monitoring. Detect gas leaks in real time, control inventory, track deliveries, and improve safety and logistics through a centralized web platform.

* **Keywords:**
  Gas cylinder monitoring, gas leak detection, LPG management system, IoT gas sensors, gas inventory control, gas distribution tracking, real-time gas alerts, gas logistics platform

---

### Meta Tags

* **Viewport:** width=device-width, initial-scale=1.0
* **Charset:** UTF-8
* **Author:** Scripters Team
* **Robots:** index, follow
* **Language:** en-US, es-ES

---

## 4.2.4. Searching Systems

### Navigation by Categories

* Navigation bar with access to the main modules:
  **Dashboard, Inventory, Alerts, Distribution, Reports, and Collections**

* Clear classification between:

    * Safety
    * Operational control
    * Logistics

* Separation by roles:

    * Company
    * Distributor
    * Supervisor

This facilitates access according to the user type.

---

### Content Search

* **FAQ Section:**
  Resolves questions about gas monitoring and platform usage.

* **Internal Search Engine:**
  Allows users to locate cylinder records, deliveries, or alerts.

* **Anchored Navigation:**
  Quick access within the dashboard to specific modules.

* **Filterable History:**
  Filters by:

    * Dates
    * Cylinder status
    * Incident type

---

## 4.2.5. Navigation Systems

### Main Navigation Bar

* Fixed horizontal (**sticky**) navigation with access to all modules
* Direct access to the **General Dashboard** with key metrics
* Highlighted button: **“View Alerts”** as a priority action

---

### Call-to-Action (CTA) Buttons

* **Dashboard:**

    * “View Details”
    * “Monitor Now”

* **Inventory:**

    * “Register Entry”
    * “Register Exit”

* **Distribution:**

    * “Track Delivery”

* **Alerts:**

    * “Handle Alert”

* **Forms:**

    * “Save”
    * “Register”

* **Color usage:**

    * Red → Alerts
    * Blue → Main actions
    * Green → Confirmations

---

### Footer Navigation

* Organized links:
  **Company, Support, Legal, Contact**

* Access to:

    * Technical support
    * Documentation
    * Policies

* Corporate information and copyright

---

### Trust Elements

* Security indicators:

    * “Real-time monitoring”
    * “Automatic alerts active”

* Metrics visualization:

    * Number of detected alerts
    * Reduction of losses
    * Operational efficiency

* Verifiable history for auditing

* Transparency in data related to:

    * Inventory
    * Distribution
    * Safety


# 4.3. Landing Page UI Design

The landing page of **Regula** is designed following a clear structure focused on **User Experience (UX)** and **conversion**, directly communicating the system’s value proposition.

---

## Main Structure

### Hero Section
- Main title (*value proposition*)
- Brief system description
- CTA buttons (*Call To Action*):
    - “Get Started”
    - “Learn More”
- Representative image of the system (dashboard + IoT)

---

### Problem & Solution Section
- Identification of problems:
    - Gas leaks
    - Manual control
    - Lack of traceability
- Presentation of the solution:
    - Real-time monitoring
    - Centralized web platform

---

### Features Section
Visualization in UI cards (*cards UI*) of functionalities:
- Real-time monitoring
- Inventory registration
- Delivery tracking (*tracking*)
- Automatic alerts

---

### Pricing Section
- Plans:
    - Basic
    - Standard
    - Premium
- CTA buttons:
    - “Choose Plan”

---

### Contact Section
- Contact form (*form UI*)
- Button:
    - “Send” (lead generation)

---

### Footer
- Secondary navigation links (*footer navigation*)
- Legal information
- Social media

---

## Design Aspects (UI/UX)

- **Responsive** design (adaptable to mobile and desktop)
- Intuitive navigation (*user-friendly navigation*)
- Use of functional colors:
    - Red → alerts
    - Blue → primary actions
    - Green → confirmations
- Structure based on **visual hierarchy** to facilitate reading

### 4.3.1. Landing Page Wireframe
<img src=".\assets\images\cap-04\landing-page\wireframes\landing-page-wireframes.png">

### 4.3.2. Landing Page Mock-up
<img src=".\assets\images\cap-04\landing-page\mockups\landing-page-mockups.png">


## 4.4. Web Applications UX/UI Design

The UX/UI design of the **Regula** web application is focused on facilitating **operational control, safety supervision, and gas cylinder management** in a fast and intuitive way.

---

### Application Structure (UI)

#### **Dashboard**

* Main view with key metrics (**KPIs**)
* Visualization of active alerts, inventory, and overall status

---

#### **Inventory Module**

* Gas cylinder entry and exit registration
* Data table (*data table*) with filters and search

---

#### **Alerts Module**

* Real-time notifications (*real-time alerts*)
* Classification by risk level (priority)

---

#### **Distribution Module**

* Delivery tracking (*tracking*)
* Route and location visualization

---

#### **Reports Module**

* Movement history
* Report generation for analysis

---

### UX Aspects (User Experience)

* **Intuitive interface:**
  Reduces the learning curve

* **Quick access:**
  Priority to critical functions (alerts and monitoring)

* **Efficiency:**
  Minimization of steps in frequent tasks

* **Immediate visual feedback:**
  Confirmations, errors, and real-time alerts

---

### UI Aspects (User Interface)

* **Clean design:**
  Clear visual hierarchy (*visual hierarchy*)

* **Use of functional colors:**

    * Red → critical alerts
    * Yellow → warnings
    * Green → normal states

* **Reusable components:**
  Buttons, tables, forms

* **Responsive design:**
  Adaptable to different devices

## 4.4.1. Web Applications Wireframes

**Segment: Gas Companies**

The wireframes for this segment are designed considering users such as plant supervisors and warehouse operators, prioritizing alert visibility and inventory control.

### Key Screens

* **Main Dashboard:**
  Panel with KPIs (active alerts, inventory level, sensor status).
  Highlighted section for real-time critical alerts.

* **Inventory Management:**
  Table-style view with a list of gas cylinders.
  Quick actions: *Register Entry*, *Register Exit*, *Filter*.

* **Alerts Panel:**
  List of alerts classified by priority.
  Main button: *“Handle Alert”*.

* **Operational Monitoring:**
  Monitoring view of sensors and warehouse status.

* **Reports:**
  Filterable history by dates and event type.

---

### Wireframe Characteristics

* Layout based on a **12-column grid**
* Use of **cards** to group information
* Fixed sidebar for main navigation
* Visual prioritization of critical alerts
* Consistent components throughout the application

These wireframes aim to ensure a clear, fast, and decision-oriented operational experience.

#### Segment: Gas Companies

![company-wireframes1.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-01.png)
![company-wireframes2.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-02.png)
![company-wireframes3.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-03.png)
![company-wireframes4.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-04.png)
![company-wireframes5.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-05.png)
![company-wireframes6.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-06.png)
![company-wireframes7.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-07.png)
![company-wireframes8.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-08.png)
![company-wireframes9.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-09.png)
![company-wireframes10.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-10.png)
![company-wireframes11.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-11.png)
![company-wireframes12.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-12.png)
![company-wireframes13.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-13.png)
![company-wireframes14.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-14.png)
![company-wireframes15.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-15.png)
![company-wireframes16.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-16.png)
![company-wireframes17.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-17.png)
![company-wireframes18.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-18.png)
![company-wireframes19.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-19.png)
![company-wireframes20.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-20.png)
![company-wireframes21.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-21.png)
![company-wireframes22.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-22.png)
![company-wireframes23.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-23.png)
![company-wireframes24.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-24.pngg)
![company-wireframes25.png](.\assets\images\cap-04\web-application\wireframes\company\company-wireframes-25.png)

---

## Segment: Gas Distributors

![distributor-wireframes1.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-01.png)
![distributor-wireframes2.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-02.png)
![distributor-wireframes3.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-03.png)
![distributor-wireframes4.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-04.png)
![distributor-wireframes5.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-05.png)
![distributor-wireframes6.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-06.png)
![distributor-wireframes7.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-07.png)
![distributor-wireframes8.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-08.png)
![distributor-wireframes9.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-09.png)
![distributor-wireframes10.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-10.png)
![distributor-wireframes11.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-11.png)
![distributor-wireframes12.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-12.png)
![distributor-wireframes13.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-13.png)
![distributor-wireframes14.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-14.png)
![distributor-wireframes15.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-15.png)
![distributor-wireframes16.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-16.png)
![distributor-wireframes17.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-17.png)
![distributor-wireframes18.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-18.png)
![distributor-wireframes19.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-19.png)
![distributor-wireframes20.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-20.png)
![distributor-wireframes21.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-21.png)
![distributor-wireframes22.png](.\assets\images\cap-04\web-application\wireframes\distributor\distributor-wireframes-22.png)

### 4.4.2. Web Applications Wireflow Diagrams

![Wireflow-01.png](.\assets\images\cap-04\web-application\wireflows-diagrams\wireflow-diagram-01.png)

---

### 4.4.2. Web Applications Mock-ups

#### Segment: Gas Companies

![company-mockup1.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-01.png)
![company-mockup2.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-02.png)
![company-mockup3.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-03.png)
![company-mockup4.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-04.png)
![company-mockup5.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-05.png)
![company-mockup6.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-06.png)
![company-mockup7.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-07.png)
![company-mockup8.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-08.png)
![company-mockup9.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-09.png)
![company-mockup10.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-10.png)
![company-mockup11.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-11.png)
![company-mockup12.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-12.png)
![company-mockup13.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-13.png)
![company-mockup14.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-14.png)
![company-mockup15.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-15.png)
![company-mockup16.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-16.png)
![company-mockup17.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-17.png)
![company-mockup18.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-18.png)
![company-mockup19.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-19.png)
![company-mockup20.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-20.png)
![company-mockup21.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-21.png)
![company-mockup22.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-22.png)
![company-mockup23.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-23.png)
![company-mockup24.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-24.png)
![company-mockup25.png](.\assets\images\cap-04\web-application\mockups\company\company-mockup-25.png)

#### Segment: Gas Distributors

![distributor-mockup1.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-01.png)
![distributor-mockup2.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-02.png)
![distributor-mockup3.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-03.png)
![distributor-mockup4.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-04.png)
![distributor-mockup5.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-05.png)
![distributor-mockup6.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-06.png)
![distributor-mockup7.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-07.png)
![distributor-mockup8.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-08.png)
![distributor-mockup9.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-09.png)
![distributor-mockup10.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-10.png)
![distributor-mockup11.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-11.png)
![distributor-mockup12.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-12.png)
![distributor-mockup13.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-13.png)
![distributor-mockup14.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-14.png)
![distributor-mockup15.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-15.png)
![distributor-mockup16.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-16.png)
![distributor-mockup17.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-17.png)
![distributor-mockup18.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-18.png)
![distributor-mockup19.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-19.png)
![distributor-mockup20.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-20.png)
![distributor-mockup21.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-21.png)
![distributor-mockup22.png](.\assets\images\cap-04\web-application\mockups\distributor\distributors-mockup-22.png)

### 4.4.3. Web Applications User Flow Diagrams

#### Segment: Gas Companies

![user-company.png](.\assets\images\cap-04\web-application\user-flow-diagrams\company\user-flow-company.png)

#### Segment: Gas Distributors

![user-distributor.png](.\assets\images\cap-04\web-application\user-flow-diagrams\distributor\user-flow-distributor.png)

---

# 4.5. Web Applications Prototyping

The web application prototypes for Regula were designed to validate the interaction flows defined during the UX process and to ensure that both gas companies and distributors can complete operational tasks quickly and intuitively. The prototypes simulate realistic navigation between modules such as inventory control, operational monitoring, alerts, distribution, and reports.

The interaction model follows the Information Architecture previously defined, maintaining consistency in navigation systems, labeling, and user flows. Priority was given to operational efficiency, immediate visibility of critical information, and minimizing the number of actions required to complete repetitive tasks.

The prototypes were developed for both desktop and mobile web browsers in order to validate responsive behavior and interaction continuity across devices. Desktop views prioritize data density and operational monitoring, while mobile views focus on quick actions, alerts, and simplified navigation for field operations.

---

## Main Interaction Decisions

### Navigation Structure

The prototypes use a persistent sidebar navigation on desktop devices and a collapsible hamburger navigation on mobile devices. This decision allows users to access critical modules rapidly without interrupting operational workflows.

Main navigation modules include:

- Dashboard
- Inventory
- Distribution
- Alerts
- Reports
- Sales
- Collections

---

### Interaction Principles

The interaction system was designed around the following principles:

- Immediate access to critical information
- Minimal clicks for repetitive operational tasks
- Real-time visual feedback
- Clear prioritization of alerts and incidents
- Consistency between desktop and mobile interactions

Operational actions such as registering entries, confirming deliveries, handling alerts, or viewing reports are accessible through highly visible CTA buttons positioned close to the main working area.

---

### Responsive Interaction

The prototypes adapt according to device size while maintaining interaction consistency:

- Desktop prioritizes monitoring dashboards and multi-panel visualization
- Tablet focuses on operational supervision with simplified layouts
- Mobile emphasizes quick access to alerts, deliveries, and inventory actions

---

## Desktop Web Prototype

The desktop prototype focuses on operational visibility, real-time monitoring, and management efficiency. The interface allows supervisors and operators to simultaneously monitor inventory, alerts, deliveries, and operational KPIs.

### Desktop Prototype Screenshot

<img src="./assets/images/cap-04/web-application/prototyping/desktop-web/desktop-screenshot.jpeg">

### Desktop Prototype Video

Microsoft Stream Video Link:

[View Prototype Demonstration Video on Microsoft Stream](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241a649_upc_edu_pe/IQB0gjWb60w1Rogd1knZcZSUATUlfGGySNMOaZpZvcus_qI?e=uOie0V&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

## Mobile Web Prototype

The mobile prototype was designed for distributors, drivers, and operational staff who require quick access during field operations. The mobile experience prioritizes simplified navigation, fast confirmation actions, and operational continuity.

### Mobile Prototype Screenshot

<img src="./assets/images/cap-04/prototyping/mobile/mobile-prototype.png">

---

### Mobile Prototype Video

Microsoft Stream Video Link:

[Insert Microsoft Stream Mobile Prototype Video Link Here]

---

# 4.6. Domain-Driven Software Architecture

Regula’s software architecture was designed following Domain-Driven Design principles in order to model the operational complexity of gas distribution, inventory traceability, operational monitoring, and safety management.

The architectural approach is centered around bounded contexts that represent clearly differentiated business capabilities. This separation allows each domain to evolve independently while maintaining consistency through domain events and asynchronous communication patterns.

The design process started with Big Picture EventStorming sessions, followed by Design-Level EventStorming workshops that refined aggregates, commands, events, policies, and domain relationships in greater detail.

The architecture was later represented using the C4 Model to visualize the system from different abstraction levels, including Context, Container, and Component diagrams.

---

## Identified Bounded Contexts

| Previous Name | Refined Bounded Context |
|---|---|
| Analítica, Reportes y Toma de Decisiones | Analytics & Decision Support |
| Gestión Comercial y Financiera del Distribuidor | Commercial & Financial Management |
| Gestión de Distribución y Logística | Distribution & Logistics |
| Gestión de Inventario y Movimientos | Inventory & Cylinder Tracking |
| Gestión de Seguridad y Alertas | Safety & Incident Monitoring |

---

# 4.6.1. Design-Level EventStorming

The Design-Level EventStorming sessions were conducted to progressively refine the domain model identified during the Big Picture EventStorming stage. The objective of these sessions was to achieve a deeper understanding of operational behavior, process continuity, business rules, automation flows, aggregate responsibilities, and bounded context interactions.

The workshops focused on refining domain events, organizing operational workflows, validating commands and policies, identifying system reactions, consolidating interactions between processes, and defining strategic architectural boundaries.

The sessions were organized into four iterative phases to progressively evolve the domain model from operational exploration to strategic architecture definition.

---

# Phase 1 — Domain Event Refinement

During this phase, the team refined the domain events identified during the Big Picture EventStorming sessions. The objective was to better understand operational timelines, identify business inconsistencies, detect pain points, and organize the main operational scenarios of the platform.

This phase focused primarily on event discovery and process clarification before introducing commands, policies, or architectural structures.

### Activities performed

* Unstructured operational exploration
* Timeline organization of business processes
* Identification of operational pain points
* Detection of pivotal business situations
* Refinement and validation of domain events

### Visual Modeling Elements

* 🟠 Domain Events

### Objectives of the Phase

* Refine events discovered during the Big Picture stage
* Organize operational processes
* Detect problematic scenarios
* Understand business continuity between events
* Identify operational bottlenecks and risks

---

## Analytics & Decision Support

<img src="./assets/images/cap-04/design-level-eventstorming/phase-01/analytics-decision-support.png">

## Commercial & Financial Management

<img src="./assets/images/cap-04/design-level-eventstorming/phase-01/commercial-financial-management.png">

## Distribution & Logistics

<img src="./assets/images/cap-04/design-level-eventstorming/phase-01/distribution-logistics.png">

## Inventory & Cylinder Tracking

<img src="./assets/images/cap-04/design-level-eventstorming/phase-01/inventory-cylinder-tracking.png">

## Safety & Incident Monitoring

<img src="./assets/images/cap-04/design-level-eventstorming/phase-01/safety-incident-monitoring.png">

---

# Phase 2 — Process and Behavior Modelling

In this phase, the team modeled operational behavior and system interactions by introducing commands, policies, actors, and read models. The goal was to define how users interact with the system and how the platform reacts to operational events.

This phase emphasized automation rules, business policies, and transactional behavior across operational workflows.

### Activities performed

* Definition of user commands
* Identification of actors and responsibilities
* Modeling of policies and automated reactions
* Creation of read models for operational visibility
* Validation of business rules and process behavior

### Visual Modeling Elements

* 🟢 Actors
* 🔵 Commands
* 🟠 Domain Events
* 🟣 Policies
* 🟩 Read Models

### Objectives of the Phase

* Model operational behavior
* Define business automation rules
* Refine interactions between users and the system
* Validate business policies and reactions
* Improve process consistency

---

## Analytics & Decision Support

<img src="./assets/images/cap-04/design-level-eventstorming/phase-02/analytics-decision-support.png">

## Commercial & Financial Management

<img src="./assets/images/cap-04/design-level-eventstorming/phase-02/commercial-financial-management.png">

## Distribution & Logistics

<img src="./assets/images/cap-04/design-level-eventstorming/phase-02/distribution-logistics.png">

## Inventory & Cylinder Tracking

<img src="./assets/images/cap-04/design-level-eventstorming/phase-02/inventory-cylinder-tracking.png">

## Safety & Incident Monitoring

<img src="./assets/images/cap-04/design-level-eventstorming/phase-02/safety-incident-monitoring.png">

---

# Phase 3 — Workflow and Interaction Consolidation

During this phase, the team consolidated the complete operational workflows by connecting business processes, validating dependencies, and analyzing continuity between operational scenarios.

The objective was to verify that commands, events, policies, and read models interacted consistently across the platform without operational conflicts or disconnected flows.

### Activities performed

* Validation of complete workflows
* Connection of operational processes
* Verification of dependencies between domains
* Analysis of process continuity
* Consolidation of event-driven interactions

### Visual Modeling Elements

* 🟢 Actors
* 🔵 Commands
* 🟠 Domain Events
* 🟣 Policies
* 🟩 Read Models

### Objectives of the Phase

* Validate operational continuity
* Refine interactions between processes
* Detect inconsistencies between workflows
* Consolidate operational behavior
* Prepare the model for strategic architectural refinement

---

## Analytics & Decision Support

<img src="./assets/images/cap-04/design-level-eventstorming/phase-03/analytics-decision-support.png">

## Commercial & Financial Management

<img src="./assets/images/cap-04/design-level-eventstorming/phase-03/commercial-financial-management.png">

## Distribution & Logistics

<img src="./assets/images/cap-04/design-level-eventstorming/phase-03/distribution-logistics.png">

## Inventory & Cylinder Tracking

<img src="./assets/images/cap-04/design-level-eventstorming/phase-03/inventory-cylinder-tracking.png">

## Safety & Incident Monitoring

<img src="./assets/images/cap-04/design-level-eventstorming/phase-03/safety-incident-monitoring.png">

---

# Phase 4 — Strategic Domain and Architecture Design

The final phase focused on defining the strategic structure of the platform by identifying bounded contexts, aggregates, and external system integrations.

This phase prepared the transition from operational domain modeling to software architecture design, ensuring clear domain boundaries and modular responsibilities.

### Activities performed

* Identification of bounded contexts
* Definition of aggregates and transactional consistency boundaries
* Analysis of external systems and integrations
* Validation of domain ownership and responsibilities
* Refinement of strategic architectural relationships

### Visual Modeling Elements

* 🟦 External Systems
* 🟨 Aggregates
* 📦 Bounded Contexts

### Objectives of the Phase

* Define system boundaries
* Group business logic into strategic modules
* Identify architectural domains
* Define integration points
* Prepare the architecture for implementation

---

## Analytics & Decision Support

<img src="./assets/images/cap-04/design-level-eventstorming/phase-04/analytics-decision-support.png">

## Commercial & Financial Management

<img src="./assets/images/cap-04/design-level-eventstorming/phase-04/commercial-financial-management.png">

## Distribution & Logistics

<img src="./assets/images/cap-04/design-level-eventstorming/phase-04/distribution-logistics.png">

## Inventory & Cylinder Tracking

<img src="./assets/images/cap-04/design-level-eventstorming/phase-04/inventory-cylinder-tracking.png">

## Safety & Incident Monitoring

<img src="./assets/images/cap-04/design-level-eventstorming/phase-04/safety-incident-monitoring.png">

---

# 4.6.2. Software Architecture Context Diagram

The Software Architecture Context Diagram represents Regula as a centralized platform interacting with external users and supporting systems. The objective of this diagram is to visualize the boundaries of the solution and identify the main actors and integrations involved in the operational ecosystem.

The context diagram includes gas companies, distributors, supervisors, IoT devices, notification services, and external mapping services used for operational tracking.

### Context Diagram

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/context/structurizr-109729-SistemaGasContext.png">

---

# 4.6.3. Software Architecture Container Diagrams

The Container Diagram presents the high-level structure of Regula and how responsibilities are distributed across the system. The architecture follows a modular and scalable approach aligned with Domain-Driven Design principles.

The solution is composed of web applications, backend services, IoT communication services, databases, and external integrations. Communication between containers combines synchronous REST APIs and asynchronous event-driven mechanisms.

The architecture was designed to support operational scalability, real-time monitoring, and high traceability requirements.

### Container Diagram

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/container/structurizr-109729-SistemaGasContainer.png">

---

# 4.6.4. Software Architecture Components Diagrams

The Component Diagrams provide a more detailed representation of the internal structure of each bounded context. These diagrams identify the main application components, domain services, repositories, APIs, and infrastructure responsibilities.

Each bounded context was modeled independently in order to preserve separation of concerns and maintain clear domain ownership.

---

## Analytics & Decision Support

This bounded context centralizes operational analytics, reporting, trend analysis, KPI evaluation, and decision-support capabilities.

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/component/structurizr-109729-AnaliticaYGestionOperativaComponent.png">

---

## Commercial & Financial Management

This bounded context manages distributor sales, debt tracking, collections, and financial operations associated with commercial workflows.

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/component/structurizr-109729-GestionComercialDistribuidorComponent.png">

---

## Distribution & Logistics

This bounded context coordinates delivery operations, route tracking, logistics supervision, and real-time distribution monitoring.

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/component/structurizr-109729-DistribucionYLogisticaComponent.png">

---

## Inventory & Cylinder Tracking

This bounded context is responsible for inventory control, cylinder movement traceability, warehouse operations, and stock monitoring.

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/component/structurizr-109729-InventarioYMovimientosComponent.png">

---

## Safety & Incident Monitoring

This bounded context manages IoT sensor monitoring, leak detection, operational alerts, incident handling, and safety supervision.

<img src="./assets/images/cap-04/domain-driven-software-architecture/c4-model/component/structurizr-109729-SeguridadOperacionalComponent.png">

---


# 4.7. Software Object-Oriented Design

The object-oriented design of Regula was developed to provide a modular, maintainable, and scalable software structure aligned with Domain-Driven Design (DDD) principles and the bounded contexts identified during the EventStorming sessions.

The class diagrams presented in this section describe the internal structure of the system by modeling entities, aggregates, services, repositories, interfaces, enumerations, and their relationships. Each bounded context was designed independently to preserve clear domain responsibilities and reduce coupling between modules.

The diagrams include:

* Classes and interfaces
* Attributes and methods
* Access modifiers (`public`, `private`, `protected`)
* Relationships and associations
* Multiplicity and navigability
* Aggregate boundaries and domain responsibilities

The objective of these diagrams is to represent the internal behavior of the platform and provide a solid foundation for implementation and architectural consistency.

---

# 4.7.1. Class Diagrams

## Analytics & Decision Support

This bounded context manages operational analytics, KPI generation, trend analysis, and decision-support processes based on inventory, alerts, and logistics information collected from other domains.

The class diagram includes:

* Operational analytics entities
* KPI calculation services
* Historical analysis models
* Trend evaluation components
* Reporting services
* Repository abstractions

The design prioritizes data aggregation, analytical consistency, and reporting scalability.

<img src=".\assets\images\cap-04\object-oriented-diagrams\Analítica%20y%20Toma%20de%20Decisiones%20BC%20SVG.svg">

---

## Commercial & Financial Management

This bounded context handles commercial transactions, customer balances, operational payments, debt tracking, and financial reporting processes.

The class diagram includes:

* Sales entities
* Payment and debt management
* Financial transaction services
* Customer account management
* Commercial repositories
* Validation services

The design focuses on transactional integrity, financial traceability, and operational consistency.

<img src=".\assets\images\cap-04\object-oriented-diagrams\Gestión%20Comercial%20y%20Financiera%20del%20Distribuidor%20BC%20SVG.svg">

---

## Distribution & Logistics

This bounded context is responsible for delivery management, route tracking, distribution monitoring, and operational logistics coordination.

The class diagram includes:

* Delivery management entities
* Route tracking models
* Distribution services
* Driver and vehicle coordination
* Logistics repositories
* Delivery status management

The design emphasizes operational continuity, real-time tracking, and logistics optimization.

<img src="./assets/images/cap-04/object-oriented-diagrams/Gestión%20de%20Distribución%20y%20Logística%20BS%20CVG.svg">

---

## Inventory & Cylinder Tracking

This bounded context manages the operational lifecycle of gas cylinders, including inventory registration, stock movement, cylinder status monitoring, and traceability processes.

The class diagram includes:

* Cylinder entities
* Inventory management services
* Entry and exit operations
* Stock monitoring models
* Repository interfaces
* Validation and tracking components

The design prioritizes inventory accuracy, traceability, and operational efficiency.

<img src="./assets/images/cap-04/object-oriented-diagrams/Gestión%20de%20Inventario%20y%20Movimientos%20BC%20SVG.svg">

---

## Safety & Incident Monitoring

This bounded context handles operational safety processes, gas leak monitoring, sensor management, and incident response coordination.

The class diagram includes:

* Incident monitoring entities
* Sensor management models
* Alert generation services
* Notification handling
* Safety repositories
* Monitoring policies

The design focuses on rapid incident detection, operational safety, and real-time monitoring reliability.

<img src="./assets/images/cap-04/object-oriented-diagrams/Gestión%20de%20Seguridad%20y%20Alertas%20BC%20SVG.svg">

---

# 4.8. Database Design

The database design of Regula was structured according to the bounded contexts identified during the domain analysis process. Each bounded context maintains its own persistence model to preserve autonomy, reduce coupling, and improve scalability and maintainability.

The database diagrams presented in this section describe the persistence structure of the platform, including entities, tables, relationships, foreign keys, and integrity constraints required to support operational processes.

The design follows relational modeling principles and considers:

* Domain separation by bounded context
* Referential integrity
* Data consistency
* Transactional reliability
* Scalability for operational growth
* Historical traceability
* Efficient querying for dashboards and analytics

Each database diagram reflects the persistence requirements of its corresponding business domain.

---

# 4.8.1. Database Diagrams

## Analytics & Decision Support

The database design for this bounded context stores operational metrics, analytical reports, KPI history, trend evaluations, and generated insights used for decision-making processes.

The database diagram includes:

* KPI tables
* Operational analytics records
* Historical analysis storage
* Reporting structures
* Analytical aggregation relationships

The design supports efficient reporting and long-term operational analysis.

<img src="./assets/images/cap-04/database-diagrams/analytics-decision-support-database-diagram.png">

---

## Commercial & Financial Management

This database diagram models the persistence structure for commercial operations, customer payments, debt tracking, billing processes, and financial records.

The database includes:

* Sales tables
* Payment records
* Debt management structures
* Customer financial accounts
* Transaction history relationships

The design prioritizes financial consistency and auditability.

<img src="./assets/images/cap-04/database-diagrams/commercial-financial-management-database-diagram.png">

---

## Distribution & Logistics

This bounded context database stores delivery information, operational routes, shipment tracking data, and logistics coordination records.

The database diagram includes:

* Delivery tables
* Route management records
* Distribution tracking entities
* Vehicle and driver associations
* Delivery status history

The design focuses on operational traceability and logistics monitoring.

<img src="./assets/images/cap-04/database-diagrams/distribution-logistics-database-diagram.png">

---

## Inventory & Cylinder Tracking

The database design for this bounded context manages the lifecycle and operational movement of gas cylinders across warehouses and distribution processes.

The database diagram includes:

* Cylinder inventory tables
* Entry and exit records
* Stock movement history
* Warehouse relationships
* Cylinder status tracking structures

The design guarantees inventory consistency and traceability.

<img src="./assets/images/cap-04/database-diagrams/inventory-cylinder-tracking-database-diagram.png">

---

## Safety & Incident Monitoring

This bounded context database stores operational alerts, sensor readings, incident history, monitoring events, and safety notifications.

The database diagram includes:

* Sensor management tables
* Alert records
* Incident history
* Monitoring event storage
* Notification tracking relationships

The design prioritizes real-time operational monitoring and historical incident analysis.

<img src="./assets/images/cap-04/database-diagrams/safety-incident-monitoring-database-diagram.png">

---