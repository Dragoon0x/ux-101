---
id: feedback-design
name: Feedback & System Status
domain: ux-interaction
version: 1.0.0
---
# Feedback & System Status
**Purpose:** Keep users informed about what's happening, what happened, and what they should do next — because uncertainty is the primary source of user anxiety in digital products.

Jakob Nielsen's first heuristic — visibility of system status — is first for a reason. Users who don't know what's happening feel anxious. Users who don't know if their action worked feel uncertain. Users who don't know what to do next feel lost. Feedback design addresses all three by making the system's state visible, comprehensible, and actionable at every moment.

## The Feedback Timing
Immediate feedback (0-100ms) confirms the interaction was registered — button states, hover effects, touch responses. Short-delay feedback (100ms-1s) confirms the action is processing — loading indicators, progress bars. Long-delay feedback (1s+) explains the wait and sets expectations — skeleton screens, progress percentages, time estimates.

## The Success/Failure Spectrum
Not every outcome is success or failure. Many actions produce partial success, conditional success, or success-with-warnings. "Your file was uploaded but is still processing" is neither success nor failure — it's an intermediate state that needs its own feedback design.

## The Undo Safety Net
The best feedback for destructive actions is not a confirmation dialog — it's an undo. Confirmation dialogs train users to click "OK" without reading. Undo lets users act confidently because they know mistakes are reversible. "Email moved to trash. Undo." is better UX than "Are you sure you want to delete this email?"

## When to use
Every user action needs feedback. When users report uncertainty about whether their actions worked. When the product has long processing times. When destructive or irreversible actions need to be protected.
