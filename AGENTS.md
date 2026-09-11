# AGENTS.md

## Project

This repository contains the website for **PCRAIG DIGITAL INC.**

PCRAIG DIGITAL is Paul Craig's small consulting company. It focuses primarily on government and public-interest technology work, particularly:

- technical strategy
- rapid prototyping
- AI product development
- forward-deployed engineering

The website is primarily a business-development and RFP-supporting website.

It should make PCRAIG DIGITAL look like a highly experienced specialist consultancy that can enter an ambiguous problem early, help determine the technical direction, and rapidly prove that direction through working software.

---

## Primary audience

The primary audience is:

1. government departments and agencies
2. government-focused consultancies looking for specialist technical capacity
3. organizations with complicated workflows that need technical strategy, prototyping, or AI product development
4. technical recruiters or recruiters from companies where Paul has submitted an application

The site should also make sense to ordinary private-sector organizations.

Government buyers should come away thinking:

> This person has worked in environments like ours, understands the constraints, can help us figure out what to do, and can actually build enough of the solution to prove it.

---

## Core positioning

The three most important ideas are:

1. **Technical strategy**
2. **Rapid product delivery**
3. **End-to-end engineering capability, particularly around implementing AI**

PCRAIG DIGITAL is particularly useful early in a project, when:

- the problem is still ambiguous
- business processes need to be understood
- assumptions need testing
- requirements are not yet trustworthy
- technical direction is still being established
- a prototype can prevent expensive mistakes later
- we have to use AI but we don't know how

Do not position Paul merely as an implementation developer who arrives after another consultancy has created the strategy.

Strategy and implementation should feel connected.

A useful shorthand is:

> understand → define direction → prototype → validate → build

---

## Voice

The voice should be:

- confident
- concise
- technically credible
- direct
- slightly irreverent
- human

It can occasionally be brash, but should not sound hostile, juvenile, arrogant, or like an advertising agency trying to be edgy.

Balance confidence with:

### Humour

Use occasional dry humour or understated jokes.

Do not turn every heading into a joke.

### Moral compass

Paul prefers building technology that improves services and institutions.

The site may express preferences for:

- useful public technology
- accessibility
- user needs
- open standards
- simple systems
- technology that makes people's lives easier

Avoid vague "technology for good" marketing language.

### Humility

The site can acknowledge that difficult projects begin with uncertainty.

A useful attitude is:

> We do not know everything at the start. That is why we research, prototype, test, and learn.

Confidence should come from experience and evidence rather than pretending every answer is obvious.

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

Do not invent or extrapolate metrics.

Do not change dates, quantities, organizations, technologies, or project roles.

If a desired claim is not supported by the supplied source material, flag it rather than inventing evidence.

---

## Design reference

`docs/preview.html` is the starting visual reference.

Do not reproduce it mechanically if a cleaner implementation achieves the same design intent.

The important characteristics are:

- warm off-white / beige background
- strong near-black text
- one highlighter-like accent colour
- restrained secondary accent colour
- substantial whitespace
- large but not absurd hero typography
- brutalist/editorial structure
- slightly friendlier typography than conventional neo-brutalism
- visible grid and alignment
- modest use of rules/borders
- aligned logo treatment
- numbers used as proof
- small hand-drawn / doodle-like details are welcome
- no giant decorative hero image
- project screenshots should be supporting elements, not dominate the page

The design should feel:

> public-interest consultancy × competent engineer × independent studio that has earned the right to be opinionated

It should not feel like:

- a SaaS landing page
- a generic management consultancy
- a giant digital agency
- cyberpunk
- a developer terminal
- a crypto startup
- pop-art chaos

---

## Landing-page structure

The current preferred structure is:

1. Header
2. Hero / major claim
3. Services / how the work gets done
   - 01 Technical strategy
   - 02 Rapid prototyping
   - 03 AI product development
4. Featured work
   - initially three projects
5. Quantitative proof
6. Client / organization logos
7. About Paul / PCRAIG DIGITAL
8. Contact
9. Minimal footer

Do not add sections merely to make the page longer.

This site does not need:

- a blog on launch
- testimonials unless genuine ones are supplied
- newsletter signup
- pricing
- fake team pages
- generic "our values" cards
- stock photography
- unnecessary FAQs

---

## Featured work

Initial featured projects should focus on recent work where Paul had unusually high ownership.

Likely initial projects:

1. New York State Apprenticeship Finder
2. Amicus: AI bot for a Government of Canada department
3. NOFO Builder for HHS

Short case-study pages may be added later under `/work/`.

For now, we want to just add the listing which will be a media component with a photo, title, description, etc. You can see them on the preview.html site.

---

## Technology

Keep the site technically boring.

Preferred implementation:

- semantic HTML
- CSS
- minimal or no JavaScript
- static assets

Do not introduce React, Next.js, Astro, Tailwind, a CMS, a bundler, or another framework without a concrete need.

The site should be capable of being hosted directly on GitHub Pages.

Prefer:

- `index.html`
- `styles.css`
- ordinary HTML case-study pages
- local images and SVGs

A little progressive enhancement is fine if genuinely useful.

Do not add JavaScript solely for visual effects.

---

## Accessibility

Accessibility is a first-class requirement.

At minimum:

- semantic HTML
- sensible heading hierarchy
- keyboard-accessible navigation
- visible focus states
- sufficient colour contrast
- useful alt text
- no information communicated by colour alone
- respect `prefers-reduced-motion`
- responsive layouts
- no inaccessible custom controls when native HTML will work

Target WCAG 2.2 AA.

Do not compromise accessibility to preserve a visual gimmick.

---

## Performance

The site should be extremely fast.

Prefer:

- minimal CSS
- no large JavaScript bundles
- appropriately sized images
- modern image formats where practical
- system fonts or a very small number of web-font files
- no unnecessary third-party scripts

Do not add analytics, trackers, cookie banners, or third-party embeds unless explicitly requested.

---

## Responsive behaviour

Design desktop-first if useful, but every page must work properly on mobile.

Avoid simply shrinking desktop typography.

Reflow layouts deliberately.

Check at minimum:

- ~375px mobile
- ~768px tablet
- ~1440px desktop

---

## SEO and machine-readable content

Use:

- useful `<title>` values
- sensible meta descriptions
- semantic heading structure
- canonical URLs where appropriate
- descriptive page copy rather than keyword stuffing

Eventually include:

- `/llms.txt`
- `/sitemap.xml`
- `/robots.txt`

The site should be easy for both humans and automated recruiting/procurement systems to understand.

---

## Contact

The primary conversion is intentionally simple:

`mailto:paul@pcraig.ca`

Do not build a contact form unless explicitly requested.

---

## Content editing rules

Prefer:

- short sentences
- concrete language
- specific evidence
- active voice
- plain English

Avoid:

- "innovative solutions"
- "digital transformation" unless context genuinely requires it
- "leverage"
- "synergy"
- "cutting-edge"
- "world-class"
- "passionate"
- generic consultancy filler

Do not describe ordinary software-development practices as extraordinary achievements.

Let project evidence establish credibility.

---

## Development workflow

When making significant changes:

1. inspect the existing implementation before editing
2. preserve the established design system unless the task specifically changes it
3. make the smallest coherent change
4. test responsive behaviour
5. check keyboard interaction and accessibility
6. verify links
7. avoid introducing dependencies unnecessarily

Do not refactor unrelated code while implementing a focused request.

---

## Definition of done

A change is done when:

- it works in a modern browser
- the layout works on mobile and desktop
- there are no obvious accessibility regressions
- factual claims remain supported
- no unnecessary dependency has been introduced
- the implementation remains suitable for static GitHub Pages hosting
- the design still feels like PCRAIG DIGITAL rather than a generic template