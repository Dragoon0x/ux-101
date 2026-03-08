---
id: button-design
name: Button Design
domain: ux-interaction
version: 1.0.0
---
# Button Design
**Purpose:** Design buttons that communicate clickability, importance, and function through visual treatment — the most fundamental interactive element in any interface.

Buttons are the primary mechanism for user action. Their design must communicate three things instantly: this is clickable (affordance), this is how important it is (hierarchy), and this is what it does (labeling). Every button that fails on any of these three dimensions creates friction.

## The Hierarchy System
Primary button: filled with brand color, highest visual weight. One per section maximum. Secondary button: outlined or tinted, medium visual weight. For alternative actions. Tertiary button: text-only or ghost, lowest visual weight. For minor actions. Destructive button: red, used only for irreversible actions. Each level should be visually distinct at a glance — if a user can't tell primary from secondary without reading the label, the hierarchy is broken.

## The Sizing Standard
Minimum touch target: 44x44px (Apple HIG) or 48x48dp (Material). Desktop minimum height: 36px. Comfortable default: 40px. Large/CTA: 48-56px. Padding: horizontal should be 2-3x vertical. Text size: 14px minimum, 16px for large buttons. These aren't style preferences — they're ergonomic requirements for accurate interaction.

## The State System
Every button needs 5 states: default, hover (desktop only), active/pressed, focused (keyboard), and disabled. Each state should be visually distinct. Hover: darken 10%. Active: darken 15% + reduce shadow. Focus: visible ring (2px, offset 2px). Disabled: 50% opacity + no pointer cursor. Transitions: 150ms ease between states.

## The Label Rules
Use verbs: "Save changes" not "OK." Be specific: "Delete project" not "Delete." Front-load the action word: "Save" not "Click here to save." 2-4 words maximum. Sentence case, not ALL CAPS (caps reduces readability by 10% and feels aggressive).
