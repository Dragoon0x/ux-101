---
id: content-for-mobile
name: Content For Mobile
domain: ux-content
version: 1.0.0
---
# Content For Mobile
**Purpose:** Apply content for mobile with the evidence-based rigor, craft precision, and user-centered discipline that separates products users love from products users merely tolerate — where every decision is grounded in research, tested with real users, and measurable in impact.

## Why This Matters

Words are the interface. The most beautifully designed button fails if the label is confusing. The most elegant form fails if the error message doesn't explain how to fix the problem. UX writing serves function — helping users understand where they are, what they can do, and what will happen when they do it. Every word should earn its place by helping the user accomplish their goal. Words that don't help are words that slow users down.

For content for mobile specifically, this is one of the UX decisions that compounds across every user interaction. When handled with rigor, it creates trust, reduces friction, and builds the kind of experience quality that users can't articulate but absolutely feel. When handled casually or defaulted, it creates subtle friction that accumulates into the vague sense that 'something about this product doesn't feel right.'

## The Frameworks

The UX Writing Principles: (1) Clear — use plain language, not jargon. (2) Concise — minimum words for maximum meaning. (3) Useful — tell users what they need to know, not what you want to say. (4) Consistent — same action = same words everywhere. These principles resolve most copy debates. If a label is clever but unclear, clear wins. If a message is thorough but too long, concise wins.

The Content Hierarchy: Button labels: 1-3 words, verbs ('Save changes'). Input labels: 1-4 words, nouns ('Email address'). Helper text: 1 sentence below the field ('We'll send a confirmation to this address'). Error messages: 1-2 sentences, specific ('Email must include @ and a domain'). Tooltips: 1-2 sentences, supplementary. Empty states: 1-3 sentences, guiding ('No projects yet. Create your first project to get started'). Page titles: 2-5 words. If any text exceeds these limits, it's trying to do too much.

The Error Message Formula: What happened (briefly) + What to do about it (specifically). 'This email is already registered. Try signing in instead, or use a different email.' Never: blame the user ('You entered an invalid email'). Never: be vague ('Something went wrong'). Never: use error codes ('Error 409'). The error is already frustrating — the message should reduce frustration, not add to it.

## The Rules

Use 'you' more than 'we.' Describe the user's outcome, not the system's action ('Your file was saved' not 'File write operation completed'). Active voice always ('We sent you an email' not 'An email was sent'). Sentence case, not Title Case or ALL CAPS (readability decreases 13-20% with all caps). Front-load the key information ('Save failed: check your internet connection' not 'We were unable to process your request due to a network connectivity issue'). Never use placeholder text as the only label — placeholders disappear on focus. Write for Grade 6-8 reading level for consumer products (Hemingway Editor).

For content for mobile specifically: validate with real users before committing. Internal opinions — even informed ones — predict user behavior poorly. A 5-user usability test on the specific implementation of content for mobile reveals more than a month of internal discussion about the best approach.

## Mental Models

The Inverted Pyramid (journalism): Most important information first, supporting details second, background last. Apply to every piece of interface text — if the user only reads the first line, they should get the essential message. Progressive Disclosure applied to content: show the minimum text needed for the task. Offer 'Learn more' for users who want depth. Don't front-load with paragraphs of explanation that most users won't read.

For content for mobile, the relevant mental model is: every UX decision is a hypothesis about user behavior until tested. The confidence in any design decision should be proportional to the evidence supporting it. High-evidence decisions (validated through research) deserve commitment. Low-evidence decisions (based on best practice or intuition) deserve rapid testing.

## How to Execute

**Step 1: Research.** What do we know about how users relate to this specific aspect of the experience? Check: existing user research, analytics data, support tickets, competitive analysis, and established UX principles. If the evidence is thin, conduct targeted research — even 3-5 user interviews focused on this specific area will dramatically improve decision quality.

**Step 2: Design with intention.** Apply the frameworks above to generate a specific design approach. Document the rationale: 'We chose [approach] because [evidence/principle]. The expected outcome is [measurable].' The documentation prevents the design rationale from being lost when the original designer moves on.

**Step 3: Test before building.** Prototype the approach and test with 5 users. The test should answer: can users accomplish the task? Where do they hesitate? What do they expect that isn't there? Prototype testing costs 1-2 days. Building the wrong solution costs weeks.

**Step 4: Measure after shipping.** Define the success metric before shipping (task completion rate, error rate, time-on-task, or SUS score improvement). Measure within 2 weeks of launch. If the metric doesn't improve, iterate. If it does, document the pattern for future reference.

## Real-World Application

**Consumer product (high volume, low expertise):** content for mobile must be immediately intuitive to first-time users. No learning curve is acceptable for basic tasks. Test with complete novices. If a first-time user can't accomplish the core task in 60 seconds without help, the design has failed.

**SaaS product (medium volume, growing expertise):** content for mobile must serve both new users (onboarding context) and experienced users (daily workflow). Progressive disclosure is key — show simplicity by default, reveal depth on demand. Test with both new signups and 30-day active users.

**Enterprise product (lower volume, high expertise):** content for mobile must be efficient for power users who spend hours in the product daily. Speed and information density matter more than simplicity. Test with actual domain experts — general usability testers won't reveal the issues that emerge at expert-level usage patterns.

## Case Studies

Mailchimp's voice guide: 'Fun but not silly, confident but not cocky, smart but not stodgy, informal but not sloppy, helpful but not overbearing.' These 5 pairs scaled the voice across 1000+ employees. Stripe's documentation voice: technical precision with unexpected warmth. The docs read like they were written by an engineer who genuinely wants you to succeed — conversational explanations of complex concepts, occasional humor, zero condescension. This voice is why Stripe's developer adoption rate leads the industry.

These case studies demonstrate a consistent pattern: the most successful products treat content for mobile as a strategic decision supported by research, not as a default to be accepted or a detail to be deferred.

## Common Mistakes

The biggest mistake with content for mobile is skipping user validation — designing based on best practice or personal preference without testing whether it works for the specific users of the specific product. Best practices are starting points, not conclusions. They must be validated in context.

The second mistake is designing only the happy path. content for mobile must be designed for edge cases, error states, and the full spectrum of user behavior — not just the ideal scenario that appears in the design file.

The third mistake is not measuring the impact. If you can't measure whether your implementation of content for mobile improved the experience, you can't improve it iteratively. Define the metric. Measure before and after. Learn from the delta.





### The Microcopy That Makes or Breaks Products
Microcopy — the tiny text fragments users encounter constantly — is where most products' voice falls apart:

**Button labels:** Describe the outcome, not the action. 'Save changes' > 'Submit.' 'Start free trial' > 'Continue.' Front-load the verb. 1-3 words maximum. Sentence case always.

**Error messages:** What happened + what to do. 'This email is already registered. Try signing in instead.' Never: 'Error 409.' Never: 'Invalid input.' Never: blame the user.

**Empty states:** What this area is for + how to fill it. 'No projects yet. Create your first project to start tracking work.' Never: 'No data to display.'

**Confirmations:** What happened + what's next. 'Your order has been placed. You'll receive a confirmation email within 5 minutes.' Be specific about timing.

**Placeholders:** Show format, not description. Email field: 'name@company.com' not 'Enter your email address.' Placeholders disappear on focus — never put essential info in them.

### The Localization-Ready Content Checklist
Write with translation in mind: (1) Avoid idioms ('hit the nail on the head' doesn't translate). (2) Avoid culturally specific references. (3) Account for text expansion (German is 30% longer than English, CJK may be shorter but wider). (4) Don't concatenate strings ('You have ' + count + ' messages' breaks in languages with different word order). (5) Use ICU message format for pluralization. (6) Allow for RTL layout. Content written for localization is also clearer in English — the constraints improve the writing.


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



### Quick Reference: UX Writing Formulas
**CTA buttons:** [Verb] + [Object/Outcome]. "Start free trial." "Download report." "Save changes." Never: "Submit." "Click here." "OK."
**Error messages:** [What happened] + [How to fix it]. "This email is already registered. Try signing in, or use a different email." Never: "Error." "Invalid input." "Something went wrong."
**Empty states:** [What this area is for] + [How to get started]. "No projects yet. Create your first project to start tracking work." Never: "No data." "Nothing to show."
**Confirmation:** [What happened] + [What's next]. "Your account was created. Check your email for a verification link." Be specific about timing and next steps.
**Tooltips:** [One thing the user needs to know]. 15 words maximum. Triggered on hover/focus. Dismissed on mouse-out/blur. Never: essential information (tooltips are supplementary).




### The Content Audit Framework

Before writing new content, audit existing content:

**Quantitative audit:** List every piece of content: URL, title, word count, last updated date, traffic (if available), owner. Export to a spreadsheet. Sort by last updated — content older than 12 months needs review. Sort by traffic — high-traffic, outdated content is a priority fix.

**Qualitative audit:** For each piece of content, assess: Is it accurate? Is it current? Is it useful? Is it findable? Is it written in the product voice? Does it meet accessibility standards? Score each dimension 1-5. Content scoring below 3 on any dimension needs revision or removal.

**Gap analysis:** What questions do users ask (from support tickets, search logs, interviews) that existing content doesn't answer? Every unanswered question is a content gap. Prioritize gaps by frequency (how many users ask) and impact (how much it affects their success).

**Action plan:** For each content piece: Keep (good quality, current, useful), Revise (useful but outdated or off-voice), Merge (overlapping with other content), Remove (outdated, low-traffic, no longer useful). The goal: less content, better content. Removing 30% of content while improving the rest usually increases overall content satisfaction.

### The Content Design Process

Content design is not copywriting. It's deciding what content exists, where it lives, and how it's structured before writing a single word:

**Step 1 — User need mapping.** What does the user need to know at this point in the journey? What question are they trying to answer? What decision are they trying to make? The content should serve the need, not serve the organization's desire to communicate.

**Step 2 — Content type selection.** What format best serves the need? A step-by-step guide? A comparison table? A FAQ? A video? A tooltip? Match the format to the need and the context. A user mid-checkout needs a tooltip, not a help article. A user evaluating pricing needs a comparison table, not a paragraph.

**Step 3 — Content hierarchy.** What's the most important information? That goes first and biggest. What's supporting detail? That goes second or behind a "Learn more" link. What's edge-case information? That goes in a help center, not on the page. Front-load the essential. Progressively disclose the rest.

**Step 4 — Drafting.** Write the content following the voice guidelines. Read it aloud — if it sounds unnatural, revise. Test the reading level (Hemingway Editor: aim for Grade 6-8 for consumer products). Verify that every sentence earns its place by helping the user accomplish their goal.

**Step 5 — Review.** Check against: brand voice guide (does it sound like us?), accessibility guidelines (is it readable? are alt texts useful? is the language plain?), legal review (if applicable — claims, disclaimers, compliance text), and user testing (does the content actually help users accomplish the task?).

### The Terminology Management System

Every product should have a single source of truth for terminology:

**The term registry:** A spreadsheet or database with columns: Term, Definition, When to use, When NOT to use, Alternative terms to avoid, Example in context. Every writer, designer, and developer references this registry. Example entry: Term: "workspace" | Definition: "A shared environment where a team collaborates" | Use: "Create a new workspace for your team" | Don't use: "project," "room," "space" (these mean different things in our product) | Context: "Your workspace includes all channels, files, and members."

Why this matters: inconsistent terminology creates cognitive load. If the product calls it "workspace" on one page and "project" on another, users must figure out whether these are the same thing or different things. Every inconsistency is a micro-confusion that adds up to the feeling that the product is disorganized.


## When to use

When this specific UX skill is the active design challenge. When usability testing reveals friction in this area. When analytics show user drop-off or confusion. When building a new feature that requires this consideration. When training team members on UX craft. When advocating for UX investment with stakeholders.

