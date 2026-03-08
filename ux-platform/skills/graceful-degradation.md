---
id: graceful-degradation
name: Graceful Degradation
domain: ux-platform
version: 1.0.0
---
# Graceful Degradation
**Purpose:** Apply graceful degradation with the rigor that makes it genuinely useful — grounded in user evidence, informed by established practice, and adapted to the specific product context.

## The Practice
Every platform has conventions that users have learned from millions of interactions. Violating conventions creates friction because users must learn new patterns. Following conventions reduces cognitive load. The skill is knowing which conventions are load-bearing (must follow) and which are surface-level (can adapt). Test with platform-native users to validate assumptions. For graceful degradation specifically, the implementation should be informed by research (what do users need?), constrained by principles (what does good practice say?), and validated by testing (does it actually work?). Assumptions are hypotheses until tested.

## The Context
graceful degradation behaves differently depending on product maturity, user expertise, platform conventions, and business constraints. What works for a consumer mobile app may fail for an enterprise desktop tool. What works for onboarding may hinder power users. Always consider the specific context before applying general guidance.

## The Measurement
The quality of graceful degradation should be measurable. Define success criteria before implementing: what user behavior would indicate this is working? Task completion rate, time-on-task, error rate, satisfaction score, and adoption rate are common UX metrics. If you can't measure it, you can't confirm it's working.

## When to use
When this specific UX challenge is the priority. When user research, usability testing, or analytics data indicates this area needs improvement. When building a new feature or product that requires this consideration.
