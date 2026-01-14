# individual-formative-assignment-mental-health-awareness
# MindCompass — Mental Health Awareness (One-Page Website)

MindCompass is a beginner-friendly, one-page mental health awareness website built to make key concepts easier to understand, scan, and navigate. The site explains mental health basics, introduces common challenges, shares practical stress-management techniques, and signposts trusted support resources.

Live site: https://ahmedaklak.github.io/individual-formative-assignment-mental-health-awareness/

---

## Table of contents
- [Project goals](#project-goals)
- [User stories](#user-stories)
- [Features](#features)
- [Design and UX](#design-and-ux)
- [Technologies used](#technologies-used)
- [How to run locally](#how-to-run-locally)
- [Deployment](#deployment)
- [Testing](#testing)
- [Known issues](#known-issues)
- [Future improvements](#future-improvements)
- [Credits](#credits)

---

## Project goals
- Provide a clear, beginner-friendly overview of mental health and wellbeing.
- Use a clean one-page structure so users can quickly find relevant sections.
- Maintain an organised layout across mobile, tablet, and desktop.
- Apply semantic HTML and accessibility-aware patterns where possible.

---

## User stories
### Primary user story
**As a user seeking beginner-friendly mental health information, I want clear and well-structured content, so that I can understand key concepts without difficulty.**

**Acceptance criteria**
- Information is organised using clear headings that convey structure.
- Content is easy to scan and locate using UX principles.
- HTML uses semantic structure (for example, sections and headings).
- Layout remains organised across device sizes.

**Implementation summary**
- Semantic `<section>` structure for each page area.
- Heading hierarchy to improve readability and screen-reader navigation.
- Bootstrap grid + spacing utilities to maintain alignment and responsive layout.

---

## Features
### Navigation
- Sticky top navigation bar with anchor links to each section.

### Hero section
- Background image with an overlay content panel for readability.
- Clear headline, supporting description, and primary CTAs.

### Mental Health Basics
- Short, beginner-friendly overview presented in a simple, scannable layout.

### Common Issues and Tips
- Three responsive cards (stack on small screens, 2+1 on medium, 3 across on large).
- Each card includes an image and a "Learn more" button.
- "Learn more" opens a Bootstrap modal that displays structured content (paragraphs and lists).

### Managing Stress
- Two-column layout on large screens.
- Bootstrap accordion for practical techniques.
- Supporting mini-cards for stress signals, daily habits, and when to seek support.

### Resources
- Basic list-group layout linking to trusted UK support and information services.

### Contact
- Simple contact form section with Bootstrap styling and client-side validation patterns.
- Includes name, email, topic, message, and acknowledgement checkbox.

### Favicon
- Site favicon included for browser tab branding.

---

## Design and UX
- Layout built with Bootstrap spacing and grid utilities for consistent rhythm and readability.
- Content is written to be beginner-friendly, short, and scannable.
- Cards, accordion, and modals reduce overwhelm by progressively disclosing content.
- Buttons provide clear next actions, especially for moving from the hero into the page.

---

## Technologies used
- HTML5
- CSS3
- Bootstrap 5 (CDN)
- JavaScript (vanilla) for modal content injection and small behaviours
- Git and GitHub for version control
- GitHub Pages for deployment

---

## How to run locally
You can run the site locally using any simple web server.

### Option A: VS Code Live Server
1. Install the Live Server extension.
2. Right-click `index.html` and select **Open with Live Server**.

### Option B: Python HTTP server
From the project root:
```bash
python -m http.server 8000

Deployment

This project is deployed using GitHub Pages.

General steps:

Commit and push changes to the repository.

In GitHub, go to Settings → Pages.

Set the source branch (commonly main) and the folder (commonly / (root)).

Save and wait for GitHub Pages to publish.

Testing
Manual testing

Confirm navigation anchors scroll to correct sections.

Check responsive behaviour across breakpoints:

Cards stack on mobile, 2+1 on tablet, 3 across on desktop.

Verify modals open and display the correct content from each card.

Confirm accordion expands/collapses correctly.

Confirm external links in Resources open in a new tab.

Confirm the contact form shows validation feedback when fields are missing.

Accessibility checks

Ensure headings follow a logical hierarchy.

Ensure buttons have clear labels.

Images include descriptive alt text.

Modals use accessible patterns (labelled title and readable content).

Known issues

Some HTML validators can flag ARIA usage in Bootstrap components depending on validator rules. Bootstrap patterns may require minor role adjustments to satisfy strict validators.

A browser console warning related to focus and aria-hidden can appear with modals in some environments; behaviour remains functional.

Future improvements

Add a dedicated “Affirmations” content set and optional daily rotation.

Add a real form submission provider (Formspree/Netlify Forms) for GitHub Pages.

Add a short “About this site” section clarifying scope and intent (education and signposting).

Improve typography and spacing consistency across all sections (global rhythm).

Add a footer with credits, disclaimer, and quick links.

Credits

Built by: Ahmed Aklak (project work and implementation)

Framework: Bootstrap 5

Support resources (UK): NHS Talking Therapies, Shout, Samaritans, PAPYRUS (linked in the Resources section)

Disclaimer

This website is for educational purposes and signposting only. It does not provide medical advice or diagnosis. If you are concerned about your safety or someone else’s safety, seek urgent help through local emergency services.
