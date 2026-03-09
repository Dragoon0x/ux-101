---
id: badge-design
name: Badge Design
domain: ux-visual
version: 1.0.0
---
# Badge Design
**Purpose:** Apply badge design with the evidence-based rigor, craft precision, and user-centered discipline that separates products users love from products users merely tolerate — where every decision is grounded in research, tested with real users, and measurable in impact.

## Why This Matters

Visual design for interfaces serves function first. Every visual property — color, size, weight, spacing, contrast — communicates something. The question is whether it communicates intentionally. Hierarchy (what's important), state (what's active/error/disabled), grouping (what belongs together), and brand (what personality the product has) should all be encoded in the visual layer simultaneously. When these layers conflict, the interface creates confusion that users feel as friction.

For badge design specifically, this is one of the UX decisions that compounds across every user interaction. When handled with rigor, it creates trust, reduces friction, and builds the kind of experience quality that users can't articulate but absolutely feel. When handled casually or defaulted, it creates subtle friction that accumulates into the vague sense that 'something about this product doesn't feel right.'

## The Frameworks

The 8-Point Grid: All spacing values are multiples of 8: 8, 16, 24, 32, 48, 64, 96. The 4px half-step exists for compact contexts (badge padding, icon-text gaps). Every padding, margin, and gap should be from the scale. Benefits: consistent rhythm, pixel-perfect alignment, and a shared language between design and development. One off-grid value breaks the rhythm that the eye subconsciously expects.

The Accessible Color System: Build the palette with accessibility as a constraint, not an afterthought. Every text color must pass 4.5:1 contrast against its background (WCAG AA for normal text). Large text (≥18px or ≥14px bold): 3:1. UI components: 3:1. Build a contrast matrix: test every foreground-background combination used in the product. Minimum 3 grays that pass AA: one for primary text (#1F2937), one for secondary (#4B5563), one for disabled (#9CA3AF on white).

The Type Scale System: Choose a ratio (1.2 minor third, 1.25 major third, 1.333 perfect fourth). Generate sizes from a 16px base: 10, 12, 14, 16, 20, 24, 30, 36, 48, 60, 72. Use max 5-6 sizes per screen. Body: 16px minimum always. Line height: 1.5 for body, 1.2-1.3 for headings. Line length: 50-75 characters (use max-width: 65ch). Letter-spacing: 0 for body, -0.01em to -0.025em for display sizes.

## The Rules

Never rely on color alone to convey information — 8% of males are colorblind. Always pair color with another signal (icon, text, pattern). Body text minimum: 16px on every screen, every device. No exceptions. Line length maximum: 75 characters. Center-aligned body text is unreadable in paragraphs — use left-align. Contrast minimum: 4.5:1 for normal text, period. 'Close enough' is a WCAG failure. Spacing must follow a scale — no magic numbers (13px, 17px, 22px are not on any scale). Icon size must snap to the grid (16, 20, 24, 32 — not 18 or 22).

For badge design specifically: validate with real users before committing. Internal opinions — even informed ones — predict user behavior poorly. A 5-user usability test on the specific implementation of badge design reveals more than a month of internal discussion about the best approach.

## Mental Models

Gestalt Principles in UI: Proximity (elements close together are perceived as grouped), Similarity (elements that look alike are perceived as related), Continuity (the eye follows lines and curves), Closure (the mind completes incomplete shapes), Figure-Ground (elements are perceived as either foreground or background). These are not design preferences — they're perceptual physics. Violate them and the interface feels wrong even if no one can explain why.

For badge design, the relevant mental model is: every UX decision is a hypothesis about user behavior until tested. The confidence in any design decision should be proportional to the evidence supporting it. High-evidence decisions (validated through research) deserve commitment. Low-evidence decisions (based on best practice or intuition) deserve rapid testing.

## How to Execute

**Step 1: Research.** What do we know about how users relate to this specific aspect of the experience? Check: existing user research, analytics data, support tickets, competitive analysis, and established UX principles. If the evidence is thin, conduct targeted research — even 3-5 user interviews focused on this specific area will dramatically improve decision quality.

**Step 2: Design with intention.** Apply the frameworks above to generate a specific design approach. Document the rationale: 'We chose [approach] because [evidence/principle]. The expected outcome is [measurable].' The documentation prevents the design rationale from being lost when the original designer moves on.

**Step 3: Test before building.** Prototype the approach and test with 5 users. The test should answer: can users accomplish the task? Where do they hesitate? What do they expect that isn't there? Prototype testing costs 1-2 days. Building the wrong solution costs weeks.

**Step 4: Measure after shipping.** Define the success metric before shipping (task completion rate, error rate, time-on-task, or SUS score improvement). Measure within 2 weeks of launch. If the metric doesn't improve, iterate. If it does, document the pattern for future reference.

## Real-World Application

**Consumer product (high volume, low expertise):** badge design must be immediately intuitive to first-time users. No learning curve is acceptable for basic tasks. Test with complete novices. If a first-time user can't accomplish the core task in 60 seconds without help, the design has failed.

**SaaS product (medium volume, growing expertise):** badge design must serve both new users (onboarding context) and experienced users (daily workflow). Progressive disclosure is key — show simplicity by default, reveal depth on demand. Test with both new signups and 30-day active users.

**Enterprise product (lower volume, high expertise):** badge design must be efficient for power users who spend hours in the product daily. Speed and information density matter more than simplicity. Test with actual domain experts — general usability testers won't reveal the issues that emerge at expert-level usage patterns.

## Case Studies

Stripe's visual system: a constrained palette (purple-blue gradient + clean neutrals + minimal semantic colors) applied with extreme consistency creates recognition even without the logo. Every element follows the same design language — from the marketing site to the dashboard to the documentation. Linear's visual design: dark mode as default, minimal color usage, monospace accents for technical feel, generous whitespace. Every visual choice reinforces the positioning: 'built for speed.' The visual restraint IS the brand statement.

These case studies demonstrate a consistent pattern: the most successful products treat badge design as a strategic decision supported by research, not as a default to be accepted or a detail to be deferred.

## Common Mistakes

The biggest mistake with badge design is skipping user validation — designing based on best practice or personal preference without testing whether it works for the specific users of the specific product. Best practices are starting points, not conclusions. They must be validated in context.

The second mistake is designing only the happy path. badge design must be designed for edge cases, error states, and the full spectrum of user behavior — not just the ideal scenario that appears in the design file.

The third mistake is not measuring the impact. If you can't measure whether your implementation of badge design improved the experience, you can't improve it iteratively. Define the metric. Measure before and after. Learn from the delta.





### The Dark Mode Design Checklist
Dark mode is not inverted light mode. It's a separate design system:

(1) **Surface hierarchy:** Light mode uses shadow for elevation. Dark mode uses surface lightness. Base: #121212. Level 1: #1E1E1E. Level 2: #2C2C2C. Level 3: #383838. Each step is 7-8 lightness units brighter.

(2) **Text colors:** Primary: #E0E0E0 (not pure white — #FFFFFF causes eye strain). Secondary: #9E9E9E. Disabled: #616161. Links: desaturate brand color by 10-20%.

(3) **Accent colors:** Reduce saturation 10-20% from light mode values. Fully saturated colors on dark backgrounds feel neon and aggressive.

(4) **Shadows:** Nearly invisible on dark backgrounds. Replace with 1px border at white/5% opacity for edge definition. Or increase surface lightness difference for elevation.

(5) **Images:** Consider reducing brightness 10-20% or adding a subtle dark overlay. Bright images on dark backgrounds feel glaring.

(6) **Testing:** Every component, every state, every page must be tested in dark mode separately. Automated contrast checking must run on both themes.

### The Responsive Typography System
Body text: 16px everywhere (never fluid — body must be consistent). Headings: fluid using clamp(). H1: clamp(2rem, 1rem + 3vw, 4.5rem). H2: clamp(1.5rem, 0.75rem + 2vw, 2.5rem). Line height: 1.5 for body (24px on 16px), 1.2 for headings. Line length: max 65ch (add max-width to text containers). Letter-spacing: 0 for body, -0.02em for display sizes (24px+). Test at every width from 320px to 1920px — fluid type should scale smoothly with no jarring jumps.


## The UX Practitioner's Playbook

### Rules That Apply to Every UX Decision

**Rule 1: Evidence over opinion.** Every design decision should be traceable to user research, analytics data, or established principle. 'I think users want X' is a hypothesis. 'In 8 of 12 interviews, users described needing X' is evidence. Design debates resolved by opinion produce compromises. Debates resolved by evidence produce solutions.

**Rule 2: The user's mental model trumps your information architecture.** If users expect a feature to be in Settings but you put it in Profile, you're wrong — even if your categorization makes more logical sense. The user's expectation, not your logic, determines findability. Test with card sorting and tree testing before committing to a structure.

**Rule 3: Design for the edge case, not just the happy path.** The happy path is: user has good data, makes no mistakes, and follows the expected flow. The edge case is: data is missing, the connection drops mid-action, the user makes an unexpected choice, the content is extremely long or extremely short. Products that only design the happy path feel polished in demos and broken in production.

**Rule 4: Accessibility is not optional.** 15-20% of users have disabilities. WCAG AA compliance is a legal requirement in most markets. Keyboard navigation, screen reader compatibility, sufficient contrast, and semantic HTML are the minimum bar — not the aspiration. Accessibility audited after the fact costs 10x more than accessibility designed from the start.

**Rule 5: Measure the experience, not just the output.** Task completion rate, time-on-task, error rate, and SUS score tell you whether the experience works. Feature adoption and page views tell you whether people found the feature. Both matter. The experience metrics tell you about quality. The adoption metrics tell you about reach. Quality without reach is invisible. Reach without quality is churn.

### Mental Models for UX Thinking

**The Experience Economy (Pine & Gilmore):** Users don't just consume products — they experience them. The experience includes: the first impression (onboarding), the daily use (workflows), the moments of failure (error states), and the final impression (offboarding/churn). Every touchpoint is part of the experience. The best UX considers the entire journey, not individual screens.

**The Peak-End Rule (Kahneman):** People judge an experience based on the peak moment (most intense) and the end (most recent), not the average. Design implications: create at least one peak moment of delight. Ensure the end of every flow is positive (confirmation, celebration, clear next steps). A perfect experience with a disappointing end feels disappointing. An imperfect experience with a great end feels good.

**The MAYA Principle (Raymond Loewy):** Most Advanced Yet Acceptable. Users want novelty (something better than what they have) but also familiarity (something they can understand). Design that's too novel confuses users. Design that's too familiar bores them. The sweet spot: innovative enough to feel better, familiar enough to feel usable. Push innovation on one dimension while keeping everything else familiar.

**Tesler's Law (Conservation of Complexity):** Every system has inherent complexity that cannot be removed — only transferred. The design decision is: does the complexity live in the system (more engineering effort) or in the interface (more user effort)? Good UX transfers complexity from the user to the system. The user's task should feel simple even when the underlying process is complex.

### Case Studies in UX Excellence

**Stripe's Developer Experience:** Stripe's documentation is the gold standard of UX for technical products. Key decisions: code examples that work when copy-pasted (functional, not illustrative). Language-specific SDKs with consistent APIs. Interactive API explorer. Error messages that include the solution, not just the problem. The insight: for developer tools, the documentation IS the UX — more time is spent in docs than in the dashboard.

**Duolingo's Retention Design:** Duolingo maintains ~55% Day-30 retention for a free consumer app — among the highest in any category. The UX architecture: short lessons (5 minutes), immediate progress feedback (XP and streaks), social accountability (leaderboards), loss aversion (streak freeze, hearts system), and adaptive difficulty (lessons get harder as you improve). Every UX element serves retention, not just engagement.

**Linear's Focused Design:** Linear is the fastest-growing issue tracker because the UX removes every ounce of friction from the workflow. Key decisions: keyboard-first interaction (every action has a shortcut). Command palette (Cmd+K) for any action. Opinionated defaults (one workflow, optimized, no configuration). Real-time sync with no loading states. The UX philosophy: reduce the time between intention and action to zero.



### Quick Reference: Visual Design Quality Signals
**Professional:** Consistent spacing from a scale. Consistent type from a hierarchy. Consistent color from a palette. Consistent radius across components. States designed for every interactive element. Dark mode deliberate, not inverted.
**Amateur:** Eyeballed spacing (13px here, 17px there). Multiple type scales mixed. Colors from different sources. Radius varies without reason. Only default state designed. Dark mode as afterthought.
**The 200% Zoom Test:** View every page at 200% zoom. If borders are crisp, shadows smooth, alignment precise, and spacing on-grid — the visual design is precise. If anything is off at 200%, users feel it subconsciously at 100%.




### The Color System Architecture

A production color system has more structure than a palette:

**Brand colors (2-3):** The primary and secondary brand colors. Used for: primary buttons, active states, links, brand elements. These colors carry brand identity — they should be distinctive and consistent.

**Neutral scale (8-10 shades):** From near-white to near-black. Example (Tailwind-style): 50, 100, 200, 300, 400, 500, 600, 700, 800, 900. Used for: backgrounds, text, borders, dividers. The neutral scale does 80% of the visual work — it creates hierarchy, separation, and depth.

**Semantic colors (4):** Success (green), Warning (amber/yellow), Error (red), Info (blue). Each needs 3 shades: light (for backgrounds), base (for text/icons), dark (for emphasis). Used for: validation states, alerts, badges, status indicators. These must be distinct from brand colors to avoid confusion between "brand element" and "status indicator."

**Extended palette (optional):** For data visualization, categorization (tag colors), or product theming. Each extended color needs the same 3-shade treatment as semantic colors. Limit to 6-8 additional colors — more creates visual noise.

**The contrast matrix:** Every text color must be tested against every background it might appear on. Build a matrix: rows = text colors, columns = background colors, cells = contrast ratio. Any cell below 4.5:1 (normal text) or 3:1 (large text) is a failure. Fix before shipping.

### The Spacing System Decision Framework

Why 8px base? Because: it divides evenly into common screen resolutions (1920, 1440, 1024, 768, 375 — all divisible by 8 or close). It creates visible-but-not-jarring increments. It's small enough for fine control and large enough for clear visual steps.

**The spacing scale applied:**
- **4px:** Minimum spacing. Icon-text gap. Badge padding. Use sparingly — it's tight.
- **8px:** Compact spacing. Form field internal padding. Related element gap. Dense UI.
- **16px:** Standard spacing. Component padding. Content paragraph gap. The default.
- **24px:** Comfortable spacing. Section padding in compact contexts. Card internal padding.
- **32px:** Section spacing. Gap between card groups. Major content sections within a page.
- **48px:** Page section spacing. Header/footer padding. Major section dividers.
- **64px:** Large section spacing. Hero padding. Major layout gaps.
- **96px+:** Extra-large spacing. Landing page sections. Premium/luxury spacing.

**The "when in doubt, add space" rule:** White space is the cheapest way to increase perceived quality. Dense interfaces feel complex. Spacious interfaces feel premium. If the design feels cluttered, the first fix is more space — before removing content, before reorganizing, before redesigning.

### The Icon Design Principles for UI

Icons in UI must be functional, not artistic:

1. **Recognition over recall.** Users should instantly recognize what the icon means without reading a label. If the icon needs a label to be understood, the icon alone isn't working — but include the label anyway (belt and suspenders).

2. **Consistency within the set.** All icons in the product should share: the same stroke weight (1.5-2px is standard), the same style (all outlined OR all filled — never mixed), the same optical size (icons should appear the same size even if pixel dimensions differ), and the same level of detail.

3. **Size snapping.** Icons should be designed at and displayed at: 16px (inline with text), 20px (in buttons and navigation), 24px (standard UI), 32px (featured/large contexts). Between these sizes, icons should scale from the nearest designed size, not be designed at arbitrary sizes.

4. **Touch target independence.** The icon is 24px. The touch target is 44px. The visual size and the interaction size are different. Pad icons with invisible touch area — not visible padding that pushes layout.


## When to use

When this specific UX skill is the active design challenge. When usability testing reveals friction in this area. When analytics show user drop-off or confusion. When building a new feature that requires this consideration. When training team members on UX craft. When advocating for UX investment with stakeholders.

