---
id: spacing-and-layout-systems
name: Spacing & Layout Systems
domain: ux-visual
version: 1.0.0
---
# Spacing & Layout Systems
**Purpose:** Create consistent, harmonious spacing across every screen — the invisible grid that makes an interface feel organized rather than assembled.

Spacing is the most undervalued visual design tool. It creates grouping (the Gestalt principle of proximity), establishes hierarchy (more space around important elements), and provides rhythm (consistent spacing creates visual order). Most interfaces have inconsistent spacing because designers eyeball it instead of systematizing it.

## The Spacing Scale
Like type, spacing works best as a scale. A base unit (typically 4px or 8px) with multiplied increments (4, 8, 12, 16, 24, 32, 48, 64, 96). Constraining spacing to the scale prevents the 13px-here-17px-there inconsistency that makes interfaces feel rough. Every padding, margin, and gap should come from the scale.

## The Density Spectrum
Different products need different density levels. A data-heavy enterprise dashboard needs tight spacing to fit more information. A consumer app needs generous spacing for touch targets and breathing room. The spacing scale stays the same — the default values shift along the density spectrum.

## The Component Spacing Model
Components have internal spacing (padding between content and edges) and external spacing (margins between components). Separating these concerns creates components that work correctly regardless of where they're placed. Internal spacing is the component's responsibility. External spacing is the layout's responsibility.

## When to use
When building a design system. When an interface feels cramped or scattered. When different designers are producing inconsistently spaced work. When implementing responsive design and spacing needs to adapt across breakpoints.
