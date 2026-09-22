---
name: toss-flow-design
description: "Design or improve mobile apps and responsive web apps using a Toss-inspired flow system: persistent navigation, summary-first home screens, card-based information hierarchy, one clear action per context, progressive disclosure, and trustworthy feedback. Use for user flows, information architecture, wireframes, UI specifications, prototypes, or frontend implementation across service domains. Do not use to copy Toss branding, proprietary assets, or screens pixel-for-pixel."
---

# Toss-style Mobile Flow Design

Turn a service into a mobile-first product that feels simple even when its underlying workflow is complex. Generalize the interaction logic; never imitate Toss trademarks, copy, illustrations, icons, or exact layouts.

## Start from the user's job

Identify the user's most frequent job, urgent or high-consequence job, information needed before acting, smallest action that creates visible progress, and actions that require review, confirmation, or recovery.

If the domain is unfamiliar or high-stakes, verify its real constraints before designing. Preserve the user's chosen platform, technology, and business model.

## Build the product spine

Create a stable mobile navigation model with 3–5 destinations. Prefer a summary-first home, one destination per recurring job, a create/capture destination when creation is central, and a catch-all area for infrequent settings and secondary services.

Label destinations with the user's nouns or verbs, not internal department names. On responsive web, keep the same conceptual destinations while adapting navigation placement to viewport size.

## Shape each screen

- Lead with the current state or next useful action.
- Use large cards to group one topic, decision, or status.
- Give each card one dominant action; demote alternatives.
- Use strong title, concise explanation, and clear status hierarchy.
- Show summaries first and reveal detail through drill-down or “view all.”
- Keep persistent navigation stable across primary destinations.
- Personalize with recent, relevant, or unfinished work when data permits.
- Introduce new or promotional content without blocking core work; always provide dismiss or later.
- Confirm consequential actions and show immediate, specific feedback.
- Provide loading, empty, error, offline, permission-denied, success, and recovery states.

Avoid turning every item into a card. Use lists for repeated homogeneous records, cards for grouped summaries or decisions, and full-screen steps for focused input.

## Adapt the pattern to the domain

Read [references/domain-adaptation.md](references/domain-adaptation.md) when translating the system into a new industry or when deciding navigation labels, trust patterns, and primary actions.

## Design input flows

- Ask only what is needed for the next decision.
- Group fields by user intent, not database structure.
- Show progress when there are multiple meaningful steps.
- Prefer device-native capture for camera, audio, location, and files.
- Preserve drafts and make interruption recovery obvious.
- Validate near the field and keep entered data after errors.
- Place review before irreversible submission.

## Trust and accessibility

- Distinguish view, edit, submit, pay, publish, and delete actions visually and verbally.
- Never use urgency, rewards, or personalization to obscure cost, consent, or risk.
- Do not expose personal or sensitive information unnecessarily in summaries or screenshots.
- Use adequate contrast, scalable text, touch targets of roughly 44 CSS pixels or larger, semantic controls, keyboard support, and visible focus.
- Do not rely on color alone for status.

## Deliverable

For planning or design work, provide a navigation map, primary and recovery paths, screen inventory, content hierarchy, component rules, state matrix, responsive behavior, assumptions, and validation questions.

For implementation, translate the same model into routes, components, state, and real responsive behavior. Reuse an existing design system when present instead of replacing it.

## Review before handoff

Check that a first-time user can identify where they are, what matters now, what the main action does, and how to recover. Ensure secondary features do not crowd the home screen, navigation labels remain stable, promotional surfaces are dismissible, and sensitive actions include proportionate confirmation.

