---
id: panel-design
name: Panel Design
domain: ux-interaction
version: 1.0.0
---
# Panel Design
**Purpose:** Apply panel design with the evidence-based rigor, craft precision, and user-centered discipline that separates products users love from products users merely tolerate — where every decision is grounded in research, tested with real users, and measurable in impact.

## Why This Matters

Interaction design is how the product feels in the moment of use — not how it looks, but how it responds. Every interaction has four components: trigger (what the user does), rules (what determines the response), feedback (what the user perceives), and loops/modes (how the system state changes). Designing all four — not just the happy path — is what separates products that feel responsive and trustworthy from products that feel unpredictable and fragile.

For panel design specifically, this is one of the UX decisions that compounds across every user interaction. When handled with rigor, it creates trust, reduces friction, and builds the kind of experience quality that users can't articulate but absolutely feel. When handled casually or defaulted, it creates subtle friction that accumulates into the vague sense that 'something about this product doesn't feel right.'

## The Frameworks

Fitts's Law: Time to reach a target = a + b × log2(D/W + 1), where D = distance and W = target width. Practical implications: make frequently-used targets large and close to the user's current position. Place primary CTAs in the thumb zone on mobile. Make destructive actions small and distant from primary actions. Infinite edges (screen edges) are the fastest targets — use them for menus and navigation.

The Interaction Design Foundation: (1) Discoverability — can users figure out what actions are possible? (2) Feedback — does the system confirm the action was received? (3) Conceptual Model — does the user's mental model match the system's behavior? (4) Affordances — do interactive elements look interactive? (5) Signifiers — do visual cues indicate how to interact? (6) Constraints — do limitations prevent errors? (7) Mapping — does the relationship between controls and effects make sense? (Norman's 7 Principles). Audit every interaction against all 7.

Microinteraction Design (Dan Saffer): Every microinteraction has 4 parts: Trigger (what initiates it — user action or system condition), Rules (what happens — the logic), Feedback (what the user sees/hears/feels — the response), Loops & Modes (what happens over time — does it change?). Example: a toggle switch. Trigger: tap. Rules: state flips. Feedback: visual position change + color change + haptic buzz. Loop: state persists until next trigger. Designing all 4 parts produces polished interactions. Missing any produces confusion.

## The Rules

Every action must have visible feedback within 100ms. No silent failures — if something goes wrong, the user must know. Undo should be available for every reversible action. Dangerous actions (delete, send, purchase) need confirmation. Hover states must not carry essential information (hover doesn't exist on mobile). Loading states must show progress, not just activity. Keyboard navigation must work for every interactive element. Touch targets must be 44x44px minimum (Apple) or 48x48dp (Material). Animation duration: 150-300ms for UI transitions, never over 500ms.

For panel design specifically: validate with real users before committing. Internal opinions — even informed ones — predict user behavior poorly. A 5-user usability test on the specific implementation of panel design reveals more than a month of internal discussion about the best approach.

## Mental Models

The Gulf of Execution and Evaluation (Norman): Gulf of Execution — the gap between the user's intention and the actions available. Gulf of Evaluation — the gap between the system's state and the user's understanding of that state. Good interaction design minimizes both gulfs: make the right action obvious (execution) and make the system's response unmistakable (evaluation). Hick's Law: Decision time increases logarithmically with the number of choices. Reduce choices at each decision point. A dropdown with 50 items is unusable — group, filter, or paginate.

For panel design, the relevant mental model is: every UX decision is a hypothesis about user behavior until tested. The confidence in any design decision should be proportional to the evidence supporting it. High-evidence decisions (validated through research) deserve commitment. Low-evidence decisions (based on best practice or intuition) deserve rapid testing.

## How to Execute

**Step 1: Research.** What do we know about how users relate to this specific aspect of the experience? Check: existing user research, analytics data, support tickets, competitive analysis, and established UX principles. If the evidence is thin, conduct targeted research — even 3-5 user interviews focused on this specific area will dramatically improve decision quality.

**Step 2: Design with intention.** Apply the frameworks above to generate a specific design approach. Document the rationale: 'We chose [approach] because [evidence/principle]. The expected outcome is [measurable].' The documentation prevents the design rationale from being lost when the original designer moves on.

**Step 3: Test before building.** Prototype the approach and test with 5 users. The test should answer: can users accomplish the task? Where do they hesitate? What do they expect that isn't there? Prototype testing costs 1-2 days. Building the wrong solution costs weeks.

**Step 4: Measure after shipping.** Define the success metric before shipping (task completion rate, error rate, time-on-task, or SUS score improvement). Measure within 2 weeks of launch. If the metric doesn't improve, iterate. If it does, document the pattern for future reference.

## Real-World Application

**Consumer product (high volume, low expertise):** panel design must be immediately intuitive to first-time users. No learning curve is acceptable for basic tasks. Test with complete novices. If a first-time user can't accomplish the core task in 60 seconds without help, the design has failed.

**SaaS product (medium volume, growing expertise):** panel design must serve both new users (onboarding context) and experienced users (daily workflow). Progressive disclosure is key — show simplicity by default, reveal depth on demand. Test with both new signups and 30-day active users.

**Enterprise product (lower volume, high expertise):** panel design must be efficient for power users who spend hours in the product daily. Speed and information density matter more than simplicity. Test with actual domain experts — general usability testers won't reveal the issues that emerge at expert-level usage patterns.

## Case Studies

Stripe's checkout interaction: every field validates inline as the user types (not after submission). Card number auto-formats with spaces. Card type auto-detected from first digits and shown with an icon. Expiry auto-advances to CVC after completion. The result: a checkout that feels intelligent and responsive, reducing form abandonment by 30%+ compared to standard forms. Gmail's undo send: after clicking send, a 5-second window with 'Undo' appears. This interaction acknowledges that the action might be premature and gives a safety net. The undo pattern transformed email sending from anxiety-inducing to confident. Duolingo's streak mechanism: the interaction loop (complete lesson → streak increments → notification next day → complete lesson) creates a habit loop that drives the highest retention in educational apps (~55% Day-30).

These case studies demonstrate a consistent pattern: the most successful products treat panel design as a strategic decision supported by research, not as a default to be accepted or a detail to be deferred.

## Common Mistakes

The biggest mistake with panel design is skipping user validation — designing based on best practice or personal preference without testing whether it works for the specific users of the specific product. Best practices are starting points, not conclusions. They must be validated in context.

The second mistake is designing only the happy path. panel design must be designed for edge cases, error states, and the full spectrum of user behavior — not just the ideal scenario that appears in the design file.

The third mistake is not measuring the impact. If you can't measure whether your implementation of panel design improved the experience, you can't improve it iteratively. Define the metric. Measure before and after. Learn from the delta.





### The Form Design Masterclass
Forms are where interfaces succeed or fail at collecting user input:

**Layout:** Single column for most forms (eye tracks straight down). Label above field (50ms faster scanning than left-aligned labels). Group related fields with headings (Personal Info, Payment, Shipping).

**Validation:** Inline, on blur (check when user leaves the field, not on every keystroke). Green checkmark for valid fields. Red with specific error below invalid fields. Never clear the field on error — the user needs to see what they typed to fix it.

**Optimization:** Every field removed increases completion 5-10%. Default to minimum: email-only signup > email + password > email + password + name. Defer non-essential fields to later. Pre-fill from context: city from ZIP, country from IP, name from social login.

**Accessibility:** Every input must have a <label>. Error messages must be associated with aria-describedby. Required fields must be indicated (asterisk + 'required' text, not color alone). Tab order must follow visual order. Submit button must be reachable by keyboard.

### The Loading State Hierarchy
Under 100ms: no indicator (feels instant). 100ms-1s: subtle inline indicator — spinner replacing the element, or the button showing a loading state. 1-3s: skeleton screen showing the shape of incoming content — gray boxes where text will appear, gray rectangles where images will appear. 3-10s: progress bar with estimated time remaining or step count. 10s+: background processing with notification when complete — don't keep the user waiting on screen. Each threshold requires a different design response. Using a spinner for a 10-second wait is as wrong as showing a progress bar for a 200ms transition.


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



### Quick Reference: Interaction Design Audit
For every interactive element, verify these 8 states:
1. **Default** — resting state, clearly interactive
2. **Hover** — visual change confirming the element is interactive (desktop only)
3. **Focus** — visible focus indicator for keyboard navigation
4. **Active/Pressed** — feedback that the action registered
5. **Loading** — indication that the system is processing
6. **Success** — confirmation that the action completed
7. **Error** — explanation of what went wrong and how to fix it
8. **Disabled** — clear visual distinction + tooltip explaining why

Missing any state = users will encounter a situation where the interface doesn't communicate. Every missing state is a trust erosion.




### The Animation & Motion Design System

Motion in UI is communication, not decoration. Every animation must answer: what is this telling the user?

**Transition types and their meaning:**
- **Fade** (opacity 0→1): Element entering or leaving. Duration: 150-200ms. Use for: modals, toasts, dropdown menus.
- **Slide** (position change): Spatial relationship between screens. Duration: 200-300ms. Use for: page transitions, drawers, panels. Direction encodes meaning: slide right = forward, slide left = back.
- **Scale** (size change): Emphasis or origin point. Duration: 150-250ms. Use for: button press feedback, modal open from trigger, image zoom.
- **Collapse/Expand** (height change): Revealing or hiding content in place. Duration: 200-300ms. Use for: accordions, expandable sections, search results.

**Easing curves:**
- **ease-out** (fast start, slow end): Use for elements entering the screen. Feels like arriving.
- **ease-in** (slow start, fast end): Use for elements leaving the screen. Feels like departing.
- **ease-in-out** (slow-fast-slow): Use for elements moving within the screen. Feels like repositioning.
- **linear**: Almost never use. Feels mechanical and unnatural.

**The reduced-motion requirement:** Always wrap animations in `@media (prefers-reduced-motion: no-preference)`. Users who set reduced-motion in their OS settings should see instant transitions (opacity only, no movement). This is an accessibility requirement, not an enhancement.

### The Gesture Design Grammar

Mobile gestures form a grammar that users learn from OS-level patterns:

- **Tap:** Primary action. The equivalent of click. Every interactive element must respond to tap.
- **Long press:** Secondary action or context menu. Use sparingly — it's hidden and undiscoverable. Never put essential functionality behind long press only.
- **Swipe horizontal:** Navigate between pages/tabs (left = forward, right = back) or reveal actions (swipe-to-delete, swipe-to-archive). Follow the platform convention — iOS uses swipe extensively, Material uses it differently.
- **Swipe vertical:** Scroll content (standard behavior) or pull-to-refresh (downward at top of list). Don't override standard scroll behavior.
- **Pinch:** Zoom. Only for content that benefits from zoom (images, maps, documents). Never disable pinch-to-zoom on web — it's an accessibility requirement.
- **Double tap:** Quick zoom in/out (maps, images). Don't use for other actions — the convention is strong.

**The discoverability problem:** Gestures are invisible. Users don't know they exist unless taught. Solutions: coach marks on first use, visible affordances (handle bars on drawers, delete icon revealed on partial swipe), and always provide a visible alternative for every gesture action.

### The State Machine Approach to Interaction Design

Complex interactions have multiple states. Model them as state machines to catch missing designs:

Example — a file upload interaction:
- **Idle:** Upload button visible, no file selected
- **Selecting:** File picker open
- **Validating:** File selected, checking type/size
- **Error (validation):** File rejected, error shown with reason
- **Uploading:** Progress bar, cancel option
- **Error (upload):** Network failure, retry option
- **Processing:** Server processing, indeterminate progress
- **Complete:** Success state, file preview, remove option

Every arrow between states is an interaction that needs design. Every state needs a visual treatment. Most interaction design failures occur because the designer only designed 3-4 of these 8 states — typically Idle, Uploading, and Complete — and left the error, validation, and processing states as system defaults that confuse users.


## When to use

When this specific UX skill is the active design challenge. When usability testing reveals friction in this area. When analytics show user drop-off or confusion. When building a new feature that requires this consideration. When training team members on UX craft. When advocating for UX investment with stakeholders.

