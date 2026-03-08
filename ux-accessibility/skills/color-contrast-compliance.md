---
id: color-contrast-compliance
name: Color Contrast Compliance
domain: ux-accessibility
version: 1.0.0
---
# Color Contrast Compliance
**Purpose:** Ensure every text and interactive element meets WCAG contrast requirements — the single most impactful accessibility improvement any product can make.

Color contrast failures are the most common accessibility issue on the web. WebAIM's annual survey of the top 1 million websites finds contrast issues on 83% of homepages. Fixing contrast is usually straightforward and dramatically improves readability for everyone, not just users with low vision.

## The Requirements
Normal text (<18px or <14px bold): 4.5:1 contrast ratio against background. Large text (≥18px or ≥14px bold): 3:1 contrast ratio. UI components and graphical objects: 3:1 contrast ratio against adjacent colors. These are WCAG AA minimums — AAA requires 7:1 and 4.5:1 respectively.

## The Common Failures
Light gray text on white backgrounds (the #999 on #FFF problem — ratio is only 2.8:1). Placeholder text that's too light to read (use #757575 minimum on white). Colored buttons where the text doesn't contrast with the button color. Focus indicators that don't contrast with the background. Disabled states that are invisible (they still need 3:1 contrast for the visual indicator, even if text doesn't need it).

## The Fix Process
1. Audit: run axe or Lighthouse on every page. 2. Catalog: list every failing color combination. 3. Fix: adjust the lighter color darker (usually easier than adjusting the background). 4. Verify: re-test every fix. 5. Prevent: build contrast requirements into the design system tokens so new combinations are pre-verified.

## The Tools
Figma: Stark plugin, A11y plugin. Browser: axe DevTools, WAVE. Standalone: WebAIM Contrast Checker, Colour Contrast Analyser. Design tokens: build contrast validation into the token pipeline so failures are caught at design time, not in production.
