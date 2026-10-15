# Aviran Katz

A responsive, single-page personal website. Plain HTML and CSS; no dependencies or build step.

## Preview

Run `python3 -m http.server 4173 --bind 127.0.0.1` in this directory, then open http://127.0.0.1:4173.

Deploy the directory to any static web host. `index.html` contains the copy; `style.css` contains the design. Fonts load from Google Fonts, with local system fallbacks. No analytics, cookies, or contact-form service.

## Content sources

- Supplied `Aviran-Katz.pdf`: career dates, experience, 150,000-user metric, skills, AI workflow, and email. These are CV claims, not independently audited metrics.
- https://www.sofi.coop/about-us: confirms Aviran’s development leadership role; source of `aviran.avif`, his public team portrait. Confirm permission for personal-site reuse before publishing.
- https://github.com/avirankatz: public professional profile and Sofi association.
- https://github.com/avirankatz/me/blob/main/src/components/Contact.tsx: corroborates email and LinkedIn URL. LinkedIn profile contents were not accessible without sign-in.
- https://www.sofi.coop/sofia: background on Sofi’s AI-agent offering; not used to claim personal ownership or specific client results.

Visual references: https://sofi.coop, https://drorisrael.org.il, https://jlmsparkcenter.co.il. The page keeps their warm palette and bold typography without copying their artwork. See [DESIGN-REVIEW.md](DESIGN-REVIEW.md) for the research-backed review of generic AI design patterns and the changes made.

The résumé download publishes the supplied PDF, including its phone number. Review those details before deployment.
