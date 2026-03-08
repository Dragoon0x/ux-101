---
id: wcag-aa-compliance
name: Wcag Aa Compliance
domain: ux-accessibility
version: 1.0.0
---
# Wcag Aa Compliance
**Purpose:** Meet WCAG 2.1 Level AA — the standard that most accessibility laws reference, adding 20 success criteria beyond Level A that address usability barriers, not just access barriers.

Level AA is where legal compliance and genuine usability meet. While Level A prevents complete exclusion, Level AA ensures the experience is actually usable — readable text, navigable structure, predictable behavior, and sufficient time to complete tasks.

## The Critical Level AA Requirements
Text contrast: 4.5:1 for normal text, 3:1 for large text (1.4.3). Text resizable to 200% without loss of content (1.4.4). Multiple ways to find pages — navigation + search + sitemap (2.4.5). Headings and labels are descriptive (2.4.6). Focus is visible (2.4.7). Consistent navigation across pages (3.2.3). Consistent identification of similar components (3.2.4). Error prevention for legal/financial/data submissions — review before submit (3.3.4). The status of programmatic elements can be determined by assistive technology (4.1.2).

## The High-Impact Changes
Fixing color contrast (test every text-background combination — tools: WebAIM Contrast Checker, Stark plugin for Figma). Adding visible focus indicators (never `outline: none` without a replacement). Making error messages specific and visible (adjacent to the field, not just at the top of the form). Ensuring all interactive elements have accessible names.

## The Business Case
Level AA compliance is required by ADA (US), EAA (EU), AODA (Canada), and Equality Act (UK). Non-compliance creates legal liability. Beyond legal: ~15-20% of users have disabilities. Accessible design also improves SEO, mobile usability, and overall user experience.
