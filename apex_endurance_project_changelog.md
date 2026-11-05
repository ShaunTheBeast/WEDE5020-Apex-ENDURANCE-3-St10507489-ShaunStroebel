# 📦 Apex Endurance — Comprehensive System Changelog

> **Project Name:** Apex Endurance — Multi-Role Endurance Platform  
> **Student Developer:** Shaun Stroebel  
> **Student ID:** ST10507489  
> **Repository:** `Apex-Endurance-Hub`  
> **Specification:** Keep a Changelog (v1.0.0) / Semantic Versioning (v2.0.0)

---

## 📑 Table of System Releases

| Version Tag | Release Milestone / Build Summary | Release Date | System Status |
| :--- | :--- | :--- | :--- |
| **`v4.2.0`** | **Exhaustive Multi-Page Architecture & Dual-Role Studio** | **2026-11-02** | **Production Release** |
| `v4.1.0` | 10-Route Gallery Expansion & Lightbox Modal Integration | 2026-11-02 | Staging Release |
| `v4.0.0` | Dual-Role State Controller & LocalStorage Engine | 2026-11-02 | Internal Build |
| `v3.2.0` | SEO Protocol Deployment (`robots.txt` & `sitemap.xml`) | 2026-11-01 | Internal Build |
| `v3.1.0` | Security Hardening & Relative Breakpoint Conversion | 2026-10-30 | Internal Build |
| `v3.0.0` | Modular File System Restructuring | 2026-10-25 | Core Architecture |
| `v2.1.0` | Dynamic Pace Calculator & Split Metric Math Logic | 2026-10-18 | Feature Build |
| `v2.0.0` | Client-Side AJAX Validation & Responsive Grid Breakpoints | 2026-10-10 | Feature Build |
| `v1.1.0` | Dark-Mode Palette Variables & Typography Setup | 2026-09-28 | Design Build |
| `v1.0.0` | Project Initialization & Initial Wireframe Prototype | 2026-09-15 | Prototype Build |

---

## 🚀 Detailed Release Logs

---

### `[v4.2.0]` — 2026-11-02 *(Final Production Release)*

#### 🌟 Added
* **Dedicated Multi-Page Router Structure:** Split monolithic layout into six standalone, specialized HTML documents:
  * `html/index.html` — Central Landing Gateway & Role Portal Hub.
  * `html/routes.html` — Interactive 10-Route Explorer with Live Lightbox.
  * `html/calculator.html` — Standalone Pace, Speed & Split Metric Engine.
  * `html/plans.html` — Periodization Blueprints & Persistent Equipment Checklists.
  * `html/creator.html` — Full Route Creator CRUD Studio & Management Table.
  * `html/contact.html` — Support Enquiry Gateway with Client Validation.
* **Navigation Active State Controller:** Added dynamic CSS class binding (`.nav-link.active`) across all HTML files to ensure exact tab tracking per view.
* **Comprehensive Documentation Suite:**
  * Created exhaustive `README.md` complete with math formulas, architectural breakdown, and screenshot indicators.
  * Created structured `CHANGELOG.md` detailing system evolution across 10 build versions.

#### 🛠️ Refactored & Enhanced
* **Guard Clause Defensive Logic (`script.js`):** Wrapped all page-specific DOM initializations inside explicit element existence checks to prevent JS console `TypeError` null pointer exceptions when navigating between standalone HTML pages.
* **Global Font Awesome Integration:** Updated all HTML headers to fetch FontAwesome v6.4.0 via CDN for unified UI icon rendering across buttons, badges, and route cards.

---

### `[v4.1.0]` — 2026-11-02

#### 🌟 Added
* **10 Iconic Endurance Routes Expansion (`html/routes.html`):**
  * **5 Long-Distance Running Courses:**
    1. *Berlin Marathon Course* (Berlin, Germany | 42.2 km | Urban Asphalt)
    2. *Peninsula Ultra Course* (Cape Town, South Africa | 56 km | Coastal Highway)
    3. *Boston Marathon Route* (Massachusetts, USA | 42.2 km | Suburban Asphalt)
    4. *Mont-Blanc Alpine Loop* (Chamonix, France | 50 km | Technical Singletrack)
    5. *Comrades "Up Run" Highway* (KwaZulu-Natal, South Africa | 87.7 km | Highway)
  * **5 Endurance Cycling Passes:**
    6. *Chapman's Peak Coastal Loop* (Cape Town, South Africa | 109 km | Coastal Tarmac)
    7. *Alpe d'Huez Ascent* (French Alps, France | 13.8 km | Switchback Pass)
    8. *Sa Calobra Winding Pass* (Mallorca, Spain | 68 km | Limestone Gorge Tarmac)
    9. *Stelvio High Alpine Pass* (Eastern Alps, Italy | 24.3 km | High Mountain Road)
    10. *Shimanami Kaido Sea Way* (Seto Inland Sea, Japan | 70 km | Suspension Bridge Cycle Paths)
* **Interactive Lightbox Modal Gallery:**
  * Added modal overlay markup (`#lightboxModal`) to handle high-res course photo previews.
  * Implemented click triggers (`.lightbox-trigger`) for image zooming and dynamic caption binding.
  * Added backdrop overlay closure on background click or `Escape` key trigger.

#### 🎨 Changed
* **Discipline Category Filter Bar:** Built real-time DOM filtering for `all`, `running`, and `cycling` tags with smooth opacity transitions (`transition: opacity 0.25s ease`).

---

### `[v4.0.0]` — 2026-11-02

#### 🌟 Added
* **Dual-Role User Ecosystem:** Introduced role switcher toggle (`Athlete / Traveler` vs `Route Creator & Customizer`) in the navigation bar.
* **Route Creator CRUD Studio (`html/creator.html`):**
  * **Create:** Built a comprehensive route publisher form accepting Title, Region, Sport, Distance, Elevation, Surface Type, Image URL, and Overview Notes.
  * **Read:** Rendered dynamic management table displaying published custom courses.
  * **Update:** Implemented inline `editRoute(id)` function pre-populating creator input fields.
  * **Delete:** Added `deleteRoute(id)` with confirmation prompt safety checks.
* **Persistent Gear Checklists (`html/plans.html`):** Bound checkbox toggles to `localStorage` key-value pairs (`gear_cb_[id]`).

---

### `[v3.2.0]` — 2026-11-01

#### 🌟 Added
* **Root Search Engine Optimization Assets:**
  * Configured `robots.txt` in project root specifying crawler allowances and sitemap path.
  * Configured `sitemap.xml` mapping all six HTML page endpoints with explicit priorities (`1.0` to `0.6`).

---

### `[v3.1.0]` — 2026-10-30

#### 🛠️ Security & Styling Hardening
* **Relative Breakpoint Standard:** Converted all media query values from fixed `px` to scalable `em` units (`22.5em`, `48em`, `64em`, `90em`).
* **Mobile Tap & Appearance Isolation:**
  * Applied `touch-action: manipulation` across all buttons and inputs to strip 300ms mobile touch delay.
  * Added `appearance: none; -webkit-appearance: none;` on form controls to block mobile webkit CSS styling injection.
* **Accessibility Overrides:** Integrated `@media (prefers-reduced-motion: reduce)` to disable transitions for users sensitive to motion.

---

### `[v3.0.0]` — 2026-10-25

#### 🎨 Changed
* **Modular Directory Migration:** Restructured project tree into standardized submission folders:
  ```text
  ├── html/
  ├── css/
  ├── javascript/
  ├── MEDIA/
  ├── robots.txt
  ├── sitemap.xml
  └── Documentation/
  ```

---

### `[v2.1.0]` — 2026-10-18

#### 🌟 Added
* **Pace & Split Calculation Engine (`calculator.html`):**
  * Built mathematical formulas converting distance and duration into Speed ($\text{km/h}$), Pace ($\text{min/km}$), and Halfway Split ($\text{HH:MM:SS}$).
  * Added client-side error handling for non-numeric or zero-value time inputs.

---

### `[v2.0.0]` — 2026-10-10

#### 🌟 Added
* **Contact Form AJAX Validation (`contact.html`):** Built real-time field validation enforcing name length, regex email formatting (`/^[^\s@]+@[^\s@]+\.[^\s@]+$/`), and minimum message length.
* **Fluid Container System:** Implemented dynamic text scaling utilizing CSS `clamp()` functions (`clamp(0.9375rem, 0.875rem + 0.25vw, 1.0625rem)`).

---

### `[v1.1.0]` — 2026-09-28

#### 🎨 Design System Definition
* **Dark Mode CSS Variable System:** Declared global variables for background colors (`--bg-dark: #0f172a`, `--bg-card: #1e293b`), typography (`--text-main: #f8fafc`, `--text-muted: #94a3b8`), and athletic neon accents (`--accent-orange: #ff6b00`, `--accent-cyan: #00f0ff`).

---

### `[v1.0.0]` — 2026-09-15 *(Initial Prototype)*

#### 🌟 Added
* Initial project setup with basic semantic HTML skeleton, hero layout, navbar, and core stylesheet reset rules.