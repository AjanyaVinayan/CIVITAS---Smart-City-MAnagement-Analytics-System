---
name: smart-city-frontend-design
description: Design and implement distinctive, production-grade frontend interfaces for the Municipal Smart City Complaint Management & Analytics System. Use this skill when building dashboards, civic portals, authentication pages, analytics screens, complaint workflows, or any UI component within the municipal platform. The output must avoid generic AI aesthetics and reflect intentional, civic-grade, system-level design thinking.
license: Complete terms in LICENSE.txt
---

This skill governs the creation of a visually distinctive, production-ready frontend interface for the **Municipal Smart City Complaint Management & Analytics System**.

The system is civic-tech infrastructure software. The frontend must feel official, trustworthy, modern, and purpose-built — not like a generic SaaS template.

The user will provide:
- A page (e.g., Citizen Dashboard, Admin Analytics, Complaint Form)
- A component (e.g., Complaint Card, Heatmap Panel, Status Timeline)
- A workflow (e.g., Complaint lifecycle UI)
- Or a full frontend build request

You must interpret the intent and build a polished, cohesive interface aligned with municipal governance software standards.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎯 DESIGN THINKING REQUIREMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Before writing code:

1. Understand the Context:
   - Is this for Citizen? Staff? Admin?
   - Is this analytical? Operational? Informational?
   - Is this urgent (critical complaint view) or calm (overview dashboard)?

2. Choose a Bold Aesthetic Direction:
   Pick one strong identity and commit fully.

   Examples:
   - Civic Institutional Modernism (structured, authoritative)
   - Data-Driven Command Center (dark, high-contrast dashboards)
   - Municipal Minimal (refined, typographic, grid-heavy)
   - Geo-Analytical Interface (map-centric layered layout)
   - Industrial Operations Console (structured, grid-heavy, utilitarian)
   - Public Service Transparency Portal (calm, neutral, high-clarity)

   The interface must feel:
   - Trustworthy
   - Deliberate
   - Systematic
   - Government-grade
   - Not startup-generic

3. Define Differentiation:
   What makes this unforgettable?
   - Is it a timeline visualization?
   - A layered status progression UI?
   - A heatmap dashboard?
   - A civic data command panel?

The design must be intentional — not decorative.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎨 FRONTEND AESTHETIC PRINCIPLES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Typography:
- Use strong, character-driven font pairings.
- Avoid: Inter, Arial, Roboto, generic system fonts.
- Prefer:
  - Editorial serif for headings (e.g., high-contrast serif)
  - Structured grotesk for body
  - Monospaced data font for analytics panels
- Establish hierarchy clearly:
  - Dashboard titles
  - Section labels
  - Status badges
  - Metadata fields

Color System:
- Define CSS variables for theme consistency.
- Avoid generic purple gradients.
- Civic themes preferred:
  - Deep navy + electric accent
  - Charcoal + signal orange
  - Slate + civic green
  - Off-white + municipal blue
- Use severity color logic:
  - Critical → strong red
  - High → amber
  - Medium → blue
  - Low → muted gray
- Priority visualization must be visually distinct.

Spatial Composition:
- Strong grid system.
- Clean alignment.
- Structured hierarchy.
- Allow negative space in dashboards.
- Avoid cluttered SaaS card grids.
- Use panel-based layouts for admin views.

Motion:
- Subtle but meaningful transitions.
- Status change animations.
- Staggered dashboard reveals.
- Hover states that indicate system responsiveness.
- Avoid playful bouncy motion.

Background & Depth:
- Use layered surfaces.
- Subtle noise textures for institutional tone.
- Panel borders.
- Grid overlays in analytics view.
- Avoid plain flat white layouts.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🧱 TECHNICAL IMPLEMENTATION RULES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Stack:
- React 18
- Vite
- JavaScript
- Tailwind CSS
- React Router v6
- Axios
- Recharts (for analytics)
- React Context (Auth)
- React Query (API handling)

Code must be:
- Fully functional
- Production-ready
- Modular
- Accessible (ARIA where needed)
- Responsive
- Cleanly structured

Folder Structure must follow:

frontend/
 ├── src/
 │   ├── pages/
 │   ├── components/
 │   ├── layouts/
 │   ├── context/
 │   ├── hooks/
 │   ├── services/
 │   ├── routes/
 │   ├── utils/
 │   ├── App.jsx
 │   └── main.jsx

Every design decision must support:
- Complaint lifecycle clarity
- Data readability
- Role-based distinction
- Operational efficiency

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📊 ROLE-SPECIFIC DESIGN BEHAVIOR
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Citizen UI:
- Clean
- Friendly but serious
- Clear progress tracking
- Emphasis on transparency
- Complaint timeline visualization

Staff UI:
- Operational
- Task-focused
- Assigned complaints highlighted
- Quick action buttons
- Status change workflow visible

Admin UI:
- Analytical
- Dense but readable
- KPI blocks
- Charts (pie, bar, line)
- Department comparison tables
- SLA compliance indicators
- Heatmap-ready layouts

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🚫 NEVER DO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

- No generic SaaS dashboard templates.
- No purple-on-white AI aesthetic.
- No cookie-cutter card layouts.
- No default component library look.
- No unstructured spacing.
- No decorative-only animation.
- No inconsistent color usage.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🎯 OUTPUT EXPECTATIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

When invoked, this skill must:

1. Define aesthetic direction explicitly.
2. Implement production-grade React code.
3. Use Tailwind with refined composition.
4. Include meaningful micro-interactions.
5. Apply severity & status visual logic.
6. Maintain cohesion across components.
7. Reflect civic infrastructure software quality.

The result should feel like:
A real municipal governance system — not a design experiment.

Every screen must feel intentional, stable, and system-aware.

Build with confidence and precision.
Commit to the vision.
Avoid mediocrity.
Deliver civic-grade frontend architecture.
