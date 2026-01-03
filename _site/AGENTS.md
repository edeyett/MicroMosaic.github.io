# AGENTS

## Project Snapshot
- **Stack:** Jekyll 4.4 (Ruby), SCSS partials (`_sass` + `assets/css/main.scss`), Markdown content pages.
- **Structure:** Custom layouts in `_layouts/`, partials in `_includes/`, case studies as a Jekyll collection (`_case_studies`).
- **Brand Assets:** Logos + portraits in `branding/` (`logo.png`, `portraits/3.png`, `portraits/4.png`), field guide + branding guide markdown.

## Key Styling Notes
- Fonts: native serif (`Georgia`) + sans (`Segoe UI`).
- Palette vars defined in `_sass/_variables.scss` (emerald teal, fungal gold, crimson, blackberry, etc.).
- Body uses flex column to keep footer pinned. Highlight cards use `.pop-*` classes for top borders; About page alternates borders via `.align-left` / `.align-right`.

## Content Mapping
- `index.md`: hero, About preview, selected services, case studies, CTA.
- `services.md`: three pillar descriptions + engagement models.
- `case-studies.md` + `_case_studies/` files: individual case study pages.
- `about.md`: portrait layout, philosophy, engagements, roots.
- `contact.md`: CTA info.

## Common Commands
- `bundle install` (after Ruby toolchain + gems).
- `bundle exec jekyll serve --port 4001` (port 4000 often blocked).
- `bundle exec jekyll build` for static output.

## Deployment
- Static site outputs to `_site/`. No live deployment configured yet (needs GitHub Pages, Netlify, etc.).

## Open Notes
- Sass `@import` warnings pending migration to `@use`/`@forward`.
- Contact CTA + case-study cards rely on `.cta` styles; maintain hover color pairs.
- Portraits expect transparent PNGs sized to fit `.about-photo` flex container.
