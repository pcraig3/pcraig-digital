# AGENTS.md

## Project

This repository contains the website for **PCRAIG DIGITAL INC.**

PCRAIG DIGITAL is Paul Craig's consulting practice.

The business focuses primarily on:

- technical strategy
- rapid prototyping
- AI product development
- forward-deployed engineering
- government and public-interest digital services

The website supports business development, consulting opportunities, RFPs,
and professional evaluation.

PCRAIG DIGITAL is intentionally a specialist practice. Do not present it as
a large agency or imply the existence of employees, teams, offices, or
capabilities that are not real.

---

## Audience

The primary audiences are:

- government departments and agencies
- public-interest organizations
- government-focused consultancies seeking specialist technical capacity
- organizations dealing with complicated workflows or ambiguous technical problems
- recruiters and hiring managers evaluating Paul Craig

The site should communicate that Paul:

- has substantial experience working in and with government
- can work directly with users, stakeholders, and organizational leadership
- can help determine technical direction before requirements are fixed
- can rapidly prototype and validate ideas
- is technically capable of building production software himself
- has significant practical experience building AI-enabled products

---

## Core positioning

The most important professional themes are:

1. **Technical strategy**
2. **Rapid product delivery**
3. **End-to-end engineering, particularly AI product engineering**

A useful shorthand is:

> understand → define direction → prototype → validate → build

---

## Voice

The site's voice should be:

- confident
- concise
- direct
- technically credible
- human
- occasionally irreverent

It can be opinionated, but should not sound:

- arrogant
- hostile
- juvenile
- overly sales-oriented
- like generic consultancy marketing

Humour should be dry and occasional.

Confidence should come primarily from specific experience and evidence.

The site can reflect preferences for:

- useful public technology
- accessibility
- user needs
- open standards
- simple systems
- maintainable software
- technology that improves services rather than adding unnecessary complexity

Avoid vague "technology for good" language.

---

## Factual source of truth

`docs/PaulCraig_CV.md` is the primary factual source for:

- employment
- job titles
- dates
- technologies
- project outcomes
- project metrics
- professional experience

---

## Existing site is the design source of truth

The current production HTML and CSS are the primary source of truth for the
site's visual design and structure.

Before changing design or layout:

1. inspect the existing implementation
2. understand the established visual patterns
3. preserve them unless the task explicitly asks for a design change

Do not rebuild existing components or styles from an older reference document
when the current implementation already establishes the intended behaviour.

The site should continue to feel like:

> public-interest consultancy × experienced engineer × independent studio

It should not drift toward:

- a SaaS landing page
- a generic management consultancy
- a giant digital agency
- cyberpunk / terminal aesthetics
- crypto branding
- generic startup templates

---

## Technology

Keep the site deliberately simple.

Current preferred architecture:

- semantic HTML
- CSS
- static assets
- minimal or no JavaScript
- direct GitHub Pages hosting

Do not introduce React, Next.js, Astro, Tailwind, a CMS, a bundler, a package
manager, or another framework without a concrete requirement that justifies it.

Do not add JavaScript solely for visual effects.

Prefer the simplest implementation that solves the problem.

---

## Accessibility

Accessibility is a first-class requirement.

Target WCAG 2.2 AA.

Preserve or improve:

- semantic HTML
- sensible heading hierarchy
- keyboard navigation
- visible focus states
- sufficient colour contrast
- meaningful alt text
- responsive layouts
- native HTML controls where possible
- reduced-motion preferences where motion exists

Do not compromise accessibility to preserve a visual effect.

---

## Performance

The site should remain extremely lightweight and fast.

Prefer:

- minimal HTML and CSS
- no unnecessary JavaScript
- appropriately sized images
- as few font files / weights as practical
- no unnecessary third-party resources

Do not sacrifice maintainability or accessibility for negligible performance gains.

---

## Responsive behaviour

Every page must work properly on mobile and desktop.

When making layout changes, check approximately:

- 375px
- 768px
- 1440px

Do not treat mobile as merely a scaled-down desktop layout.

---

## Content

Prefer:

- short sentences
- concrete language
- specific evidence
- active voice
- plain English

Avoid generic consultancy filler such as:

- innovative solutions
- leverage
- synergy
- cutting-edge
- world-class
- passionate

"Digital transformation" may be used deliberately or ironically, but should
not become generic marketing language.

Do not describe normal software-development practices as extraordinary
achievements.

---

## Contact

The primary conversion is:

`mailto:paul@pcraig.ca`

---

## SEO and machine-readable content

Preserve useful:

- page titles
- meta descriptions
- semantic heading structure
- descriptive content
- alt text
- canonical URLs where appropriate

The project may contain:

- `llms.txt`
- `sitemap.xml`
- `robots.txt`

These should contain factual, useful information rather than instructions
attempting to manipulate search engines or language models.

---

## Working in this repository

Before editing:

1. inspect the relevant existing files
2. understand the established implementation
3. make the smallest coherent change that satisfies the task

While editing:

- preserve existing conventions where they work
- avoid unrelated refactors
- avoid unnecessary dependencies
- do not change copy, design, or behaviour outside the requested scope without reason

After editing:

1. review the diff
2. test affected layouts at appropriate viewport sizes
3. check keyboard interaction when relevant
4. verify affected links and assets
5. check for obvious accessibility regressions
6. report material decisions, tradeoffs, or unresolved issues

---

## Definition of done

A change is complete when:

- it satisfies the requested task
- it works in modern browsers
- affected mobile and desktop layouts work
- there are no obvious accessibility regressions
- factual claims remain supported
- no unnecessary dependency has been introduced
- the site remains suitable for static GitHub Pages hosting
- the result still feels consistent with the existing PCRAIG DIGITAL site
