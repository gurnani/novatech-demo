# NovaTech Solutions

## Project Overview

NovaTech Solutions is a tech consultancy website. This project demonstrates advanced Claude Code features for the Pluralsight course.

## Tech Stack

- HTML5 semantic markup
- CSS3 with custom properties (design tokens)
- Vanilla JavaScript (ES6+ modules)
- No frameworks — intentionally simple for learning

## Project Structure

```
src/pages/     → HTML pages (index, services, portfolio, team, contact)
src/css/       → Stylesheets organized by scope
src/js/        → JavaScript modules
tests/         → E2E (Playwright) and unit tests
docs/          → Design specs and API documentation
```

## Code Conventions

### HTML
- Use semantic elements (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`)
- Include ARIA labels for accessibility
- Keep pages under 200 lines

### CSS
- Follow BEM naming: `.block__element--modifier`
- Use CSS custom properties from `variables.css`
- Mobile-first responsive design

### JavaScript
- ES6 modules with named exports
- JSDoc comments for public functions
- No global variables

## Git Workflow

- `main` — Production-ready code
- `feature/*` — New features
- `bugfix/*` — Bug fixes

Commit message format: `type: description`

Examples:
- `feat: add contact form validation`
- `fix: correct mobile nav toggle`
- `docs: update README setup instructions`

## Testing

Run tests before committing:

```bash
npm run test        # All tests
npm run test:unit   # Unit tests only
npm run test:e2e    # E2E tests only
```

## Current Focus Areas

- Accessibility improvements (WCAG 2.1 AA)
- Form validation enhancements
- Mobile navigation refinements



# Behavioral Guidelines

 

**Tradeoff:** These guidelines bias toward caution over speed. For trivial tasks, use judgment.

 

## 1. Think Before Coding

 

**Don't assume. Don't hide confusion. Surface tradeoffs.**

 

- State your assumptions explicitly. If uncertain, ask.

- If multiple interpretations exist, present them - don't pick silently.

- If a simpler approach exists, say so. Push back when warranted.

- If something is unclear, stop. Name what's confusing. Ask.

 

## 2. Simplicity First

 

**Minimum code that solves the problem. Nothing speculative.**

 

- No features beyond what was asked.

- No abstractions for single-use code.

- No "flexibility" or "configurability" that wasn't requested.

- No error handling for impossible scenarios.

- If you write 200 lines and it could be 50, rewrite it.

 

## 3. Surgical Changes

 

**Touch only what you must. Clean up only your own mess.**

 

- Don't "improve" adjacent code, comments, or formatting.

- Don't refactor things that aren't broken.

- Match existing style, even if you'd do it differently.

- Remove imports/variables/functions that YOUR changes made unused.

- Don't remove pre-existing dead code unless asked.

 

## 4. Goal-Driven Execution

 

**Define success criteria. Loop until verified.**

 

- "Add validation" → "Write tests for invalid inputs, then make them pass"

- "Fix the bug" → "Write a test that reproduces it, then make it pass"

- "Refactor X" → "Ensure tests pass before and after"


- 

