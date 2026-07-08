# TrustFix — Clickable Prototype (Week 3)

**Product Matters 6.0 · E-Cell IIT Guwahati · Product Management Course**

A functional, clickable prototype of TrustFix, a trusted home-services marketplace, built as the Week 3 deliverable: taking the Week 2 wireframes and MVP scope and turning them into an interactive walkthrough of the core customer and service-professional flows.

🔗 **Live demo:** https://product-matters-trustfix-prototype.onrender.com 

## What this is

A single-page, dependency-free HTML/CSS/JS prototype that simulates two linked mobile apps side by side in a phone-frame UI:

- **Customer app** - service discovery, professional matching, booking, live tracking, OTP-verified job start/completion, and rating
- **Professional app** - availability toggle, job request/acceptance, OTP-verified job start, in-progress job execution (photo capture + checklist), OTP-verified completion, and payout

Each screen ships with an annotation panel explaining the product reasoning behind it - what it traces back to from the Week 2 MVP, and any gaps or decisions that surfaced specifically while building (e.g. the exact sequencing of who triggers what during job completion and payout).

## Why this approach

The assignment brief calls for AI-assisted / "vibe coded" prototyping without production engineering support. Rather than a multi-screen Figma/Visily click-through, this was built as one self-contained HTML file with vanilla JS state management - no framework, no build step, no backend. It's easy to host, easy to iterate on, and forces the same interaction-design decisions a native app would (navigation, state transitions, empty/loading states) without the overhead of real infrastructure.

## Tech

- Plain HTML, CSS, and JavaScript - no framework, no bundler
- Google Fonts (Fraunces + Inter) loaded via CDN
- No backend, no database - all state is simulated in-browser and resets on refresh

## Running locally

No install needed. Either:

```bash
# Just open it
open index.html
```

or serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

Hosted on [Render](https://render.com) as a static site:
- **Build command:** none
- **Publish directory:** `.`

Any push to `main` auto-redeploys.

## Repo structure

```
.
├── index.html   # the entire prototype
└── README.md
```

## Related deliverables

- Week 2: Problem definition, personas, MVP, GTM strategy, wireframes
- Week 3 deck: "Prototyping TrustFix — From Wireframes to a Working Model" (what changed, tool & approach, revised MVP, updated metrics/risks)
