---
id: keyboard-accessibility
name: Keyboard Accessibility
domain: ux-accessibility
version: 1.0.0
---
# Keyboard Accessibility
**Purpose:** Ensure every feature works with keyboard alone — because keyboard access is the foundation of all assistive technology access, not an edge case.

If it doesn't work with a keyboard, it doesn't work with a screen reader, switch device, voice control, or any other assistive technology. Keyboard accessibility is the gateway to all other forms of access. It's also used by power users, users with temporary injuries, and anyone who prefers keyboard efficiency.

## The Tab Order
Tab order must follow visual reading order (left-to-right, top-to-bottom in LTR languages). Never use positive tabindex values (tabindex="1", "2", etc.) — they create unpredictable navigation. Use tabindex="0" to add elements to the natural tab order. Use tabindex="-1" to make elements focusable programmatically but not in the tab sequence.

## The Interaction Patterns
Buttons: activated by Enter and Space. Links: activated by Enter only. Dropdowns: Arrow keys to navigate options, Enter to select, Escape to close. Modals: Tab trapped within the modal, Escape to close, focus returns to trigger on close. Tabs: Arrow keys to switch tabs, Tab to move into tab panel content. These patterns are defined by WAI-ARIA Authoring Practices — don't invent new ones.

## The Testing Protocol
Tab through every page. Can you reach every interactive element? Can you see where focus is (visible focus indicator)? Can you activate every control? Can you escape every modal, dropdown, and overlay? Can you skip repetitive navigation (skip links)? Test without a mouse for 30 minutes. Every frustration you feel is multiplied for users who can't fall back to a mouse.
