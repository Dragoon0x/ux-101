---
id: wcag-a-compliance
name: Wcag A Compliance
domain: ux-accessibility
version: 1.0.0
---
# Wcag A Compliance
**Purpose:** Meet WCAG 2.1 Level A — the minimum legal accessibility standard that most products still fail, covering the 25 success criteria that prevent the most severe access barriers.

Level A is the floor, not the ceiling. These criteria address the most fundamental accessibility barriers — content that is completely inaccessible to entire groups of users. Failing Level A means some users literally cannot use the product at all. Every criterion represents a real person locked out.

## The Critical Level A Requirements
All images have alt text (1.1.1). All video has captions (1.2.2). Content doesn't rely on color alone to convey information (1.4.1). All functionality is keyboard-accessible (2.1.1). Users can pause, stop, or hide moving content (2.2.2). Nothing flashes more than 3 times per second (2.3.1). Every page has a descriptive title (2.4.2). Link purpose is clear from the link text (2.4.4). The language of the page is programmatically determined (3.1.1). No major parsing errors in HTML (4.1.1).

## The Common Failures
Missing alt text on images (the most common failure — audit every image). Form inputs without associated labels (use `<label for="id">`). Keyboard traps (user can tab in but can't tab out — test every modal and dropdown). Auto-playing media without pause control. Focus order that doesn't match visual order.

## The Testing Method
Run automated testing first (axe DevTools catches ~30-40% of issues). Then manual keyboard testing (tab through every page). Then screen reader testing (VoiceOver on Mac, NVDA on Windows). Automated + manual + screen reader catches ~85% of Level A issues.
