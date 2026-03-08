---
id: ui-color-system
name: UI Color System Design
domain: ux-visual
version: 1.0.0
---
# UI Color System Design
**Purpose:** Build a color system that serves function, brand, and accessibility simultaneously — not a palette, but a system with roles, rules, and governance.

Color in interfaces is functional before it's aesthetic. Color communicates state (error, success, warning), creates hierarchy (primary actions vs secondary), groups related elements, and signals brand identity. A color system organizes these functions into a coherent architecture that scales across the product.

## The Semantic Layer
Colors should be named by function, not by appearance. "Primary action" not "blue-500." "Error" not "red." "Surface elevated" not "gray-100." Semantic naming means the system can be re-skinned, themed, or adapted for dark mode without restructuring — because the function stays constant even when the visual implementation changes.

## The Accessibility Foundation
WCAG AA requires 4.5:1 contrast for normal text and 3:1 for large text. These are minimums, not goals. Build the color system with accessibility baked in — every text-on-background combination should be pre-verified. Don't leave accessibility to individual designers checking one-off combinations.

## The Dark Mode Architecture
Dark mode is not inverted light mode. It requires a separate color architecture with different surface hierarchies, different elevation models, and different accent color treatments. The semantic layer makes this manageable — the same functional tokens map to different visual values in light and dark modes.

## When to use
When building a design system. When the product has inconsistent color usage. When implementing dark mode. When accessibility audit reveals contrast failures. When the brand colors need to work harder in the interface.
