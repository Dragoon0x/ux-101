---
id: error-message-writing
name: Error Message Writing
domain: ux-content
version: 1.0.0
---
# Error Message Writing
**Purpose:** Write error messages that help users fix the problem — specific, visible, actionable, and never blaming the user.

Most error messages fail because they describe what went wrong in system terms instead of telling the user what to do in human terms. "Invalid input" is a system description. "Email must include @ and a domain (e.g., name@company.com)" is a human instruction.

## The Error Message Formula
What happened (briefly) + What to do about it (specifically). "This email is already registered. Try signing in instead, or use a different email." Not: "Error 409: Conflict." Not: "That didn't work. Please try again." The user needs to know what failed AND how to succeed.

## The Tone Rules
Never blame the user: "You entered an invalid date" → "Please enter a date in MM/DD/YYYY format." Never be vague: "Something went wrong" → "We couldn't save your changes. Check your internet connection and try again." Never be dramatic: "FATAL ERROR" → "We're having trouble loading this page. Refresh to try again." The error is already frustrating — the message should reduce frustration, not add to it.

## The Placement Rules
Inline validation errors appear directly below the field, in red (#DC2626), with a warning icon. Form-level errors appear at the top of the form AND next to the specific fields. Toast/banner errors for system issues appear at the top of the viewport. Error messages should remain visible until the error is resolved — never auto-dismiss error messages.
