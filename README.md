# AiTHOS Health Passport — Teen Acquisition Page

Mobile-first teen acquisition page. Single conversion goal: get a 13–17-year-old from "interested" to "Passport built, parent link sent" in under 90 seconds.

## What this is

A focused replacement for the prior Health Passport landing page when the goal is **teen acquisition specifically** — direct-response, mobile-first, conversational onboarding via SAiRA, with the Passport visibly assembling as the teen answers questions.

This page is intentionally narrow. It does **not** explain the product to parents, providers, or investors. Each of those audiences should have its own page (`/parents`, `/providers`, `/about`) rather than competing for space on the teen conversion path.

## Design principles

- **Mobile-first.** The shell is sized for a phone canvas; desktop is a wider phone, not the other way around.
- **The Passport is visible above the fold.** The product the teen is signing up for is on screen before they read anything else.
- **SAiRA is the form.** Instead of a static form, signup is four conversational questions with one-tap answers and a "name your name" text prompt. The Passport fills in as each answer comes in — completeness percentage rises, stats light up, the card pulses on each update.
- **Parent comes after, not during.** The teen never sees "invite a parent" as a signup step. The parent-completion link is the *closing action* of the flow, framed as "send your parent the details link" rather than "your parent has to sign you up."
- **No records required to begin.** Surfaced in the hero meta and reiterated in SAiRA's framing.

## Files

- `index.html` — single-file static page (HTML + CSS + JS inline)
- `README.md` — this file

Deploys to GitHub Pages from the repo root. No build step.

## What's prototype-only

- Apple Wallet add — placeholder modal; production needs real PassKit pass generation
- Parent completion link send — placeholder modal; production needs the SAiRA-mediated link generation flow
- No data persistence — state lives in memory only
- No analytics or capture — add when ready

## Sibling pages to build next

The strategic decision called out in this product line is to **split the audiences**: this page serves teens; `/parents` should serve parents (legitimacy, fiduciary architecture, completion-to-conversion path); `/providers` should serve clinics (the AiTHOS Certified Provider concept, the records-release flow, the SAiRA-mediated link mechanic).

Confidential concept material — Cadence Cove LLC.
