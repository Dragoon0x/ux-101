---
id: research-repository
name: Research Repository
domain: ux-research
version: 1.0.0
---
# Research Repository
**Purpose:** Apply research repository with the evidence-based rigor, craft precision, and user-centered discipline that separates products users love from products users merely tolerate — where every decision is grounded in research, tested with real users, and measurable in impact.

## Why This Matters

UX research is the discipline of understanding users deeply enough to solve their actual problems — not the problems the team assumes they have. Research replaces opinion with evidence, assumption with observation, and debate with data. The cost of research is measured in days. The cost of building the wrong thing is measured in months. Every hour of research saves 10 hours of misguided design and development.

For research repository specifically, this is one of the UX decisions that compounds across every user interaction. When handled with rigor, it creates trust, reduces friction, and builds the kind of experience quality that users can't articulate but absolutely feel. When handled casually or defaulted, it creates subtle friction that accumulates into the vague sense that 'something about this product doesn't feel right.'

## The Frameworks

Continuous Discovery (Teresa Torres): Talk to at least one user per week as a team habit — not a quarterly research project. Use the Opportunity Solution Tree: Desired Outcome → Opportunities (user needs discovered through interviews) → Solutions (ideas that address opportunities) → Assumptions (things that must be true) → Experiments (cheap tests of assumptions). Weekly rhythm prevents the drift between team assumptions and user reality that quarterly research can't catch.

The Research Quality Pyramid: At the base: sample quality (are you talking to the right people?). Middle: question quality (are you asking the right things?). Top: synthesis quality (are you drawing the right conclusions?). Most research failures happen at the base — the team talks to convenient participants instead of representative users, and the findings don't generalize.

The 5-User Rule (Nielsen): Testing with 5 users catches ~85% of usability issues. Diminishing returns after 5 — the 6th through 15th users find progressively fewer new issues. For evaluative research (testing a specific design), 5 users per round is sufficient. For generative research (discovering new insights), 8-12 interviews typically reach saturation — hearing the same themes repeated.

## The Rules

Never ask 'would you use this?' — everyone says yes but behavior predicts nothing from hypothetical questions. Always ask about past behavior: 'Tell me about the last time you...' Never fill silence — count to 5 after every answer before asking the next question. The best insights come in the silence. Always record sessions (with consent) but take notes as if the recording doesn't exist. Note-taking forces attention. Never present findings without evidence — 'users want X' must be followed by 'because in 7 of 12 interviews, participants described Y behavior.'

For research repository specifically: validate with real users before committing. Internal opinions — even informed ones — predict user behavior poorly. A 5-user usability test on the specific implementation of research repository reveals more than a month of internal discussion about the best approach.

## Mental Models

The Double Diamond (Design Council): Diverge (explore the problem space broadly) → Converge (define the specific problem) → Diverge (explore solutions broadly) → Converge (define the specific solution). Research lives primarily in the first diamond — understanding before solving. The Mom Test (Rob Fitzpatrick): Talk about the user's life, not your idea. Ask about specific past experiences, not hypothetical futures. Listen for the emotional weight behind statements. Bad: 'Would you use an app that...?' Good: 'What happened the last time you tried to...?'

For research repository, the relevant mental model is: every UX decision is a hypothesis about user behavior until tested. The confidence in any design decision should be proportional to the evidence supporting it. High-evidence decisions (validated through research) deserve commitment. Low-evidence decisions (based on best practice or intuition) deserve rapid testing.

## How to Execute

**Step 1: Research.** What do we know about how users relate to this specific aspect of the experience? Check: existing user research, analytics data, support tickets, competitive analysis, and established UX principles. If the evidence is thin, conduct targeted research — even 3-5 user interviews focused on this specific area will dramatically improve decision quality.

**Step 2: Design with intention.** Apply the frameworks above to generate a specific design approach. Document the rationale: 'We chose [approach] because [evidence/principle]. The expected outcome is [measurable].' The documentation prevents the design rationale from being lost when the original designer moves on.

**Step 3: Test before building.** Prototype the approach and test with 5 users. The test should answer: can users accomplish the task? Where do they hesitate? What do they expect that isn't there? Prototype testing costs 1-2 days. Building the wrong solution costs weeks.

**Step 4: Measure after shipping.** Define the success metric before shipping (task completion rate, error rate, time-on-task, or SUS score improvement). Measure within 2 weeks of launch. If the metric doesn't improve, iterate. If it does, document the pattern for future reference.

## Real-World Application

**Consumer product (high volume, low expertise):** research repository must be immediately intuitive to first-time users. No learning curve is acceptable for basic tasks. Test with complete novices. If a first-time user can't accomplish the core task in 60 seconds without help, the design has failed.

**SaaS product (medium volume, growing expertise):** research repository must serve both new users (onboarding context) and experienced users (daily workflow). Progressive disclosure is key — show simplicity by default, reveal depth on demand. Test with both new signups and 30-day active users.

**Enterprise product (lower volume, high expertise):** research repository must be efficient for power users who spend hours in the product daily. Speed and information density matter more than simplicity. Test with actual domain experts — general usability testers won't reveal the issues that emerge at expert-level usage patterns.

## Case Studies

Slack discovered through research that teams didn't want a 'communication tool' — they wanted to reduce the anxiety of not knowing what was happening across the company. This insight shaped the product: searchable history, channels for transparency, and integrations that centralized notifications. Instagram's founders spent weeks interviewing users of Burbn and discovered people only used the photo-sharing feature — the discovery led to killing 80% of the product and one of the most successful pivots in tech history. Spotify's Discover Weekly emerged from research showing users wanted to discover new music but were overwhelmed by choice — the insight was that curation, not catalog size, was the value.

These case studies demonstrate a consistent pattern: the most successful products treat research repository as a strategic decision supported by research, not as a default to be accepted or a detail to be deferred.

## Common Mistakes

The biggest mistake with research repository is skipping user validation — designing based on best practice or personal preference without testing whether it works for the specific users of the specific product. Best practices are starting points, not conclusions. They must be validated in context.

The second mistake is designing only the happy path. research repository must be designed for edge cases, error states, and the full spectrum of user behavior — not just the ideal scenario that appears in the design file.

The third mistake is not measuring the impact. If you can't measure whether your implementation of research repository improved the experience, you can't improve it iteratively. Define the metric. Measure before and after. Learn from the delta.





### The Research Repository That Compounds
After every research project, extract: (1) Key findings (3-5 bullet points). (2) Verbatim quotes that capture the insight. (3) Tags (product area, user segment, method, date). (4) Confidence level (strong/moderate/emerging). (5) Implications for design. Store in a searchable repository (Dovetail, Airtable, or Notion). After 20 research projects, the repository becomes the most valuable asset the UX team owns — a searchable memory of everything learned about users. The repository prevents: re-researching topics already studied, losing institutional knowledge when researchers leave, and the 'we did research but I can't find it' problem.

### The Research Ops Fundamentals
Research operations (ReOps) makes research scalable: (1) Participant panel — a pre-screened, recruitable database of users segmented by characteristics. Invest in building this once; use it for every study. (2) Consent and privacy — standardized consent forms, data handling procedures, and GDPR/privacy compliance. Set up once, never worry again. (3) Research tools — standardized tool stack (recording tool, analysis tool, repository tool). (4) Templates — interview guide template, survey template, usability test script template, synthesis template. Each template embeds best practices so every researcher — even junior ones — produces consistent quality. (5) Scheduling — automated participant scheduling (Calendly or similar) with reminders. Manual scheduling is the biggest time waste in research ops.


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



### Quick Reference: Research Method Cheat Sheet
**Need to discover unknown problems?** → User interviews (8-12 participants, 45 min each)
**Need to test a specific design?** → Usability test (5 users, task-based, think-aloud)
**Need to validate information architecture?** → Tree test (50+ users) or card sort (15-20 users)
**Need to measure satisfaction?** → SUS survey (20+ users, post-task)
**Need to understand behavior at scale?** → Analytics + session recordings (1000+ users)
**Need to find what matters most?** → Top tasks survey (200+ users)
**Have 1 day?** → Guerrilla usability test (5 users, coffee shop or hallway)
**Have 1 hour?** → Expert heuristic review (Nielsen's 10 heuristics, one reviewer)
**Have 5 minutes?** → The squint test (blur your eyes — can you see the hierarchy?)




### The Insight Extraction Method

Raw research data is not insight. The gap between data and insight is where most UX research fails. Here's the systematic method for crossing that gap:

**Step 1 — Capture verbatim.** After each interview, extract 15-25 verbatim quotes that carry emotional weight or reveal behavior. Not paraphrases — the exact words. The language users choose reveals mental models that paraphrases destroy. When a user says "I feel stupid every time I try to use this" that's fundamentally different from the researcher writing "user found the interface confusing."

**Step 2 — Code the data.** Apply tags to each quote: behavior (what they do), motivation (why they do it), pain (what frustrates them), workaround (how they compensate), and emotion (how they feel about it). After coding 50-100 quotes across 8-12 interviews, patterns emerge that no single interview could reveal.

**Step 3 — Build affinity clusters.** Group coded quotes into themes. The themes should emerge from the data, not from your expectations. If you went in looking for "onboarding problems" but the data clusters around "trust and transparency," follow the data. The clusters ARE the insights — they represent the patterns of real user behavior that your design must address.

**Step 4 — Write insight statements.** Structure: "[User group] needs [need] because [motivation], but currently [barrier], which results in [consequence]." Example: "New users need to understand pricing before signing up because they've been burned by hidden costs before, but the current pricing page requires a login to see details, which causes 40% to bounce before ever creating an account." Each statement is actionable — it points directly to a design solution.

**Step 5 — Prioritize by impact.** Not all insights are equal. Rank by: frequency (how many users mentioned this), severity (how much does it affect their experience), and solvability (can we actually fix this). A frequent, severe, solvable problem is the highest priority. A rare, mild, difficult problem is the lowest.

### The Research Bias Checklist

Before trusting any finding, check for these 7 common biases:

1. **Confirmation bias** — did you only notice data that supports what you already believed? Counter: have someone who disagreed with your hypothesis review the same data independently.

2. **Sampling bias** — did you only talk to one type of user? Counter: verify demographic/behavioral diversity in your participant pool. If all 8 interviewees are power users, your findings don't represent new users.

3. **Social desirability bias** — did users tell you what they thought you wanted to hear? Counter: ask about past behavior, not future intentions. Observe actions, not just words.

4. **Recency bias** — are you overweighting the last interview because it's freshest in memory? Counter: synthesis should happen after ALL sessions, not incrementally after each one.

5. **Leading question bias** — did your questions steer the answer? Counter: review your interview guide for leading language. "Don't you think this is confusing?" is leading. "How would you describe this experience?" is neutral.

6. **Survivorship bias** — did you only study current users and miss the users who already left? Counter: include churned users and non-users in your participant pool when studying adoption or retention.

7. **Anchoring bias** — did an early data point set an expectation that colored everything after? Counter: randomize the order you review data. Start synthesis from the full dataset, not from the first interview.

### The Stakeholder Research Presentation Formula

Research that doesn't change decisions is wasted research. The presentation structure that drives action:

**Opening (2 min):** "We talked to [N] users over [timeframe] to answer the question: [specific research question]." State the question. Stakeholders need to know what to listen for.

**Key findings (10 min, max 5 findings):** Each finding: the insight statement + 2-3 supporting quotes + data visualization if quantitative. Play a 30-second video clip of a real user struggling. Video clips move stakeholders more than any amount of bullet points. One clip of a user failing at the checkout flow is worth 50 slides of analytics.

**Implications (5 min):** For each finding: "This means we should [specific action]." Connect every finding to a concrete next step. If a finding doesn't have an implication, cut it — it's interesting but not actionable.

**Discussion (15 min):** "What surprised you? What do you disagree with? What questions do you have?" The discussion reveals whether stakeholders will act on the findings. If they're resistant, address the objections now — not after you've designed a solution they'll reject.

The 30-minute format is intentional. Research presentations longer than 30 minutes lose stakeholder attention. If you have more to share, put it in an appendix and send it after the meeting.


## When to use

When this specific UX skill is the active design challenge. When usability testing reveals friction in this area. When analytics show user drop-off or confusion. When building a new feature that requires this consideration. When training team members on UX craft. When advocating for UX investment with stakeholders.

