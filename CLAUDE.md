You are a senior product designer + frontend engineer.
Build a stunning, investor-ready marketing website for “HOPE”. It must clearly explain the product to non-technical people and impress experts.

Brand & Style

Logo: text-only — HOPE in bold (no icon).

Palette: dark navy #0A2540 (primary), royal blue #1E40AF (accents), off-white #F9FAFB (background), charcoal #111827 (text), subtle gray #E5E7EB (borders).

Typography: Inter (or similar), large headings, generous white space.

Vibe: premium healthcare, trustworthy, calm, ultra-professional.

Tech & Behavior

Stack: Next.js + React, Tailwind CSS, Framer Motion for smooth scroll-triggered animations, shadcn/ui components, lucide-react icons.

Interactions: sticky top navbar with active-section highlighting; section reveal on scroll (fade/slide/parallax), hover states on cards and CTAs; smooth in-page anchors.

Performance/SEO: responsive, accessible (WCAG AA), semantic HTML, meta tags / OpenGraph, favicons.

Page Structure (single-page with anchored sections)

Hero

Big “HOPE” logo, concise tagline, sub-headline, primary CTA (“Get Updates”) and secondary CTA (“Contact Sales”).

App-store area: “Coming soon to App Store and Google Play” with realistic store badge visuals (SVGs as placeholders).

What is HOPE (Plain-English)

3-4 short bullets explaining the value in human terms (no jargon).

One illustrative graphic (SVG mock) showing “You → Watch & Phone → HOPE → Guidance”.

How HOPE Works (Step Flow)

4 steps with icons & short copy:
(1) Intake (Onboarding Questionnaire + Interactive LLM Intake) →
(2) Data (Wearable/Device Integration: Apple Watch, Fitbit, BP cuffs via SpikeAPI-like connectors) →
(3) AI Insights (Risk Scoring; Provisional Diagnostic Suggestions clearly labeled “requires physician confirmation”; Baseline Comparison vs similar cohorts) →
(4) Action (Doctor Recommendations; next steps & education).

Patient-Facing Features (cards with hover)

Onboarding Questionnaire; Interactive LLM Intake; Wearable Integration; Risk Scoring (Low/Med/High); Provisional Suggestions (with safety label); Baseline Comparison; Doctor Recommendations; Educational Explanations.

Clinician & Partner Features

Structured Patient Summaries (LLM-generated for EHRs), Outcome Tracking (post-treatment monitoring), Performance Scoring (adjusted for compliance), API Access (expose HOPE+ models as endpoints for telehealth/insurers/pharma; knowledge access only, no raw patient data).

Technology & Security

HIPAA-aligned cloud stack (S3 storage, SageMaker training/deploy, API Gateway delivery), encryption in transit/at rest, de-identification, audit logging.

Multimodal data fusion (ECG, labs, vitals, symptoms, wearables).

Feedback loop for continuous learning; scalable deployment for consumer + B2B.

Pricing (elegant 3-tier table with toggles and hover emphasis)

Basic — personal insights, standard updates.

Pro — advanced insights, longitudinal trends, priority support.

Enterprise / API — model API access, SSO, SLA, compliance docs, sandbox keys, volume-based pricing, dedicated support.

CTA buttons: “Get Pro” and “Contact Sales for Enterprise”.

FAQs (accordion) — simple answers for non-technical users (privacy, accuracy, what devices, “Does HOPE replace doctors?” → No).

Call-to-Action

“Be first to try HOPE” email capture (client-side only; wire the form to a mailto: or placeholder function with a success toast).

Footer

Contact, social, legal links.

Copy Guidelines (generate concise, investor-impressive text)

Use plain language first, then a one-liner for experts under each section.

Clearly state HOPE is assistive and does not replace physicians.

Be explicit that Enterprise/API provides access to models/intelligence, not raw PHI.

Deliverables

Fully working Next.js project (TypeScript).

Files & structure:

pages/index.tsx (or app/page.tsx) with all sections and anchors.

components/ → Navbar.tsx, Hero.tsx, HowItWorks.tsx, FeaturesPatient.tsx, FeaturesClinician.tsx, Technology.tsx, Pricing.tsx, FAQs.tsx, CTA.tsx, Footer.tsx.

lib/animations.ts for Framer Motion variants; lib/copy.ts for key strings.

public/assets/ for SVGs (app-store badges, phone mockups, logos).

styles/globals.css (Tailwind base + small overrides).

README.md with run instructions: npm i && npm run dev.

Implement scroll-triggered animations (Framer Motion) on each section with tasteful durations/easing, not flashy.

Constraints

No data collection beyond a simple email placeholder; no PHI.

No external APIs required (use local SVGs/placeholders).

Must look premium on desktop and mobile; avoid clutter.

Start by printing a brief PLAN (sections, components, and animation approach). Then scaffold the project and implement.