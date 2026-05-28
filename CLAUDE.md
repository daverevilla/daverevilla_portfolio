# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static portfolio website for Dave Revilla, UX Research Strategist. Plain HTML, CSS, and a small amount of JavaScript. No build tools, no frameworks, no bundlers. Based on specific design mocks.

## Stack

- **Languages:** HTML, CSS, JavaScript (minimal — mobile menu toggle only)
- **Fonts:** Inter (body) + Fraunces (headings) via Google Fonts
- **Hosting:** Render (free static site tier)
- **Domain:** Registered at Squarespace, DNS pointed at Render
- **Version control:** Git + GitHub

## Design Specs

- **Colors:** Charcoal #2D2D2D, Warm white #FAF9F6, Accent teal #3A8D8C, Light gray #E0E0E0, Dark gray text #555555
- **Fonts:** Fraunces (h1/h2, 700 weight), Inter (body/nav/buttons, 400/600 weight)
- **Layout:** Max-width 1200px container, centered. CSS Grid for card layouts, Flexbox for nav/alignment.

## File Structure

```
index.html          — Homepage (hero, featured work cards, about teaser, footer)
work.html           — Work page (all case study cards in a grid)
case-study.html     — Case study detail template (one page, reused per project)
about.html          — About page (bio, photo, skills, contact CTA)
styles/main.css     — All styling
scripts/main.js     — Mobile nav toggle only
images/             — Project thumbnails and photos
```

## Deployment

Every `git push` to `main` triggers automatic redeploy on Render (continuous deployment). Publish directory is `.` (repo root).

## Build Schedule (from guide)

- **Day 1:** Environment setup, create index.html skeleton with semantic HTML, link CSS file, first git commit
- **Day 2:** Build homepage — nav, hero section, featured work cards, about teaser, footer. All HTML structure first, then CSS.
- **Day 3:** Build Work page and Case Study page — grid of cards, detail page with sections
- **Day 4:** Build About page, add all internal navigation links, connect pages together
- **Day 5:** Responsive design — mobile nav, media queries, flexible images
- **Day 6:** Deploy to Render, connect custom domain
- **Day 7:** Polish — hover effects, transitions, final review, content updates

## Claude Code Usage Rules

**This is a learning project. Claude Code must act as tutor and debugger, NOT as a code generator.**

- NEVER write HTML, CSS, or JavaScript code for the user
- Explain concepts when asked (e.g., "what does display: flex do?")
- Debug errors when the user pastes code or error messages — explain what's wrong and why
- Review code the user has written and suggest improvements with explanations
- Always explain fixes line by line; don't just hand over solutions
- If the user asks you to build, add, or write code for them, remind them of the learning rules
