---
id: tooltip-design
name: Tooltip Design
domain: ux-interaction
version: 1.0.0
---
# Tooltip Design
**Purpose:** Design tooltips that provide context without interrupting the task — the smallest and most frequently misused UI element.

Tooltips are for supplementary information — content that helps but isn't required. The moment a tooltip contains essential information (the only place a user can learn what a button does), the design has failed. Essential information should be visible without interaction.

## The Trigger Rules
Desktop: show on hover after a 300-500ms delay (prevents tooltips firing during casual mouse movement). Hide on mouse leave after 100ms delay (prevents flicker). Touch: show on long-press, hide on tap-away. Never show tooltips on tap — it conflicts with the element's primary action.

## The Content Rules
Maximum 1-2 short sentences. No titles in tooltips (that's a popover). No interactive content in tooltips (links, buttons — that's a popover). No images. The tooltip should be readable in 2-3 seconds. If the content requires more time, it should be a popover or inline help.

## The Positioning
Place tooltips above the trigger element by default. Flip to below if above would go off-screen. Never cover the element that triggered the tooltip. Arrow pointing to the trigger element, centered on the trigger. 8px gap between tooltip and trigger. Max width: 240px to prevent tooltips from becoming paragraphs.
