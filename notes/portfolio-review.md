# Portfolio Review Log

Last updated: 2026-04-14

## Context

This repository contains a single-file portfolio site in `portfolio.html`, based on Hardik Gulati's resume and linking to GitHub and LinkedIn.

The initial request was:
- review the portfolio
- find loose ends
- recommend improvements
- ask before making changes

## Initial Review Findings

Main issues identified in the first review pass:

1. Projects had no proof links or calls to action.
- The site described projects well, but there were no links to GitHub, demos, or case studies.

2. Mobile navigation disappeared entirely.
- The fixed desktop sidebar was hidden on small screens and there was no mobile replacement.

3. Resume and portfolio content were inconsistent.
- `SecureBytes` appeared on the site, while the resume used `FraudGuard`.
- `NexaKind` dates required confirmation.

4. No resume download link was present.
- The PDF existed in the repo, but the site did not link to it.

5. Recruiter-facing metadata was missing.
- No meta description
- No social sharing metadata
- Minimal accessibility support

6. One metric felt inflated.
- The hero said `5+ Projects` while exactly 5 projects were listed.

## User Clarifications

Confirmed by the user:
- `FraudGuard` is the correct project name
- `NexaKind` date is `Aug 2025 to Nov 2025`

## Technical Changes Implemented

Changes made in `portfolio.html` during the technical cleanup pass:

1. Metadata improvements
- Added `meta description`
- Added `theme-color`
- Added Open Graph tags
- Added basic Twitter card tags

2. Accessibility improvements
- Added a skip link
- Added visible focus styles
- Added `aria-current` handling for active navigation links
- Added reduced-motion handling with `prefers-reduced-motion`

3. Mobile navigation
- Added a sticky mobile navigation bar
- Added mobile section links
- Updated scroll tracking so active section state works for both desktop and mobile nav

4. Resume access
- Added resume links in:
  - desktop sidebar
  - mobile nav
  - contact section

5. Content consistency fixes
- Renamed `SecureBytes` to `FraudGuard`
- Kept `NexaKind` as `Aug 2025 — Nov 2025`
- Changed `5+ Projects` to `5 Projects`

## Current Recommendations

Recommended next improvements, in priority order:

1. Improve the hero section
- Make it clearer what role Hardik is targeting
- Tighten the one-line positioning
- Optimize for recruiter scanning in 5 seconds

2. Add project proof links
- GitHub
- demo
- case study
- or `available on request` for private work

3. Create project hierarchy
- Feature the strongest 2-3 projects more prominently
- Keep the weaker/supporting projects secondary

4. Sharpen project copy
- Add stronger impact statements
- Add real metrics where available
- Make ongoing vs completed work clearer

5. Improve contact conversion
- Replace generic contact copy with direct recruiter-facing messaging
- Mention target roles such as:
  - AI/ML Intern
  - Data Science Intern
  - Analytics Intern

6. Refine skills grouping
- Group by hiring relevance, for example:
  - Languages
  - ML / Data
  - Backend
  - Tools

7. Add small polish items later
- favicon
- social preview image
- optional project thumbnails for top work

## Working Agreement From This Chat

Current workflow established in this session:
- review first
- ask before major changes
- apply approved changes directly in code
- keep a written summary in the repo for continuity

## Note On Future Updates

This file can be updated as the portfolio evolves. In the current session, it should be treated as the running log of:
- decisions
- completed changes
- pending recommendations
