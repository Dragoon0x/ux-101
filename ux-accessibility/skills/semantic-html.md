---
id: semantic-html
name: Semantic Html
domain: ux-accessibility
version: 1.0.0
---
# Semantic Html
**Purpose:** Use HTML elements for their meaning, not their appearance — because semantic HTML is the foundation that makes assistive technology, SEO, and maintainability work.

Semantic HTML means using `<nav>` for navigation, `<button>` for actions, `<a>` for links, `<h1>`-`<h6>` for headings in order, `<main>` for primary content, `<article>` for self-contained content, and `<section>` for thematic grouping. This is not academic — screen readers use these elements to build a page outline that users navigate, search engines use them to understand content, and developers use them to write maintainable code.

## The Critical Distinctions
`<button>` vs `<div onClick>`: A button is keyboard-accessible, focusable, activatable by Enter and Space, and announced as "button" by screen readers. A div with an onClick handler does none of these things. Never build a custom button from a div — the accessibility cost is immense. Links go somewhere (`<a href>`). Buttons do something (`<button>`). Using one for the other confuses both assistive technology and users.

## The Heading Hierarchy
Headings must be hierarchical: one `<h1>` per page, `<h2>`s under it, `<h3>`s under `<h2>`s. Never skip levels (jumping from `<h2>` to `<h4>`). Screen reader users navigate by headings — 67.5% of screen reader users say headings are their primary navigation method (WebAIM survey). A page with broken heading hierarchy is a page with broken navigation for screen reader users.

## The Landmark Regions
`<header>`, `<nav>`, `<main>`, `<aside>`, `<footer>` create landmark regions that screen readers can jump between. A page with these landmarks lets a screen reader user skip directly to navigation, main content, or footer without tabbing through everything. Every page should have at least `<main>` and `<nav>`.
