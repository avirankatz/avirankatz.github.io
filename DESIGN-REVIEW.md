# Review: generic AI design patterns

## Research

Read on 15 October 2026:

- [Anthropic: Frontend Design](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md). Practitioner guidance, not an empirical study. Identifies identical rounded cards, single-word headline accents, numbered markers without a sequence, uppercase eyebrows, repeated arrows, and interchangeable copy as common generated-design defaults. Also warns that replacing them with a fashionable editorial template merely creates another default.
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing). A community-maintained advice page, primarily for encyclopedic writing, not a formal policy or a landing-page study. Its observations about generic praise, repeated three-part constructions, and negative parallelisms are useful editing prompts here. The page explicitly cautions that style is not proof of AI authorship.

Google, DuckDuckGo, and Brave search presented bot challenges; Bing returned irrelevant results. The findings above are from directly retrieved sources, not purported search consensus.

## Assessment

The previous page’s problem was cumulative: almost every section used the same marketing cadence and decorative devices. The palette and large type fit the user's references; they were not problems to remove just because they are fashionable. The correction is to make the content and hierarchy specific to Aviran, rather than attempt to disguise how the site was made.

### Identity and copy — `index.html`

| Before | After |
| --- | --- |
| “Good code. Better impact.” and generic impact-oriented metadata | Aviran’s name, actual role, and specific professional description in the hero, title, and metadata |
| “Developer. Architect. Human.” and “Building everywhere” | Removed unnecessary identity labels and unsupported global framing |
| Repeated “thoughtful,” “purpose,” “people first,” and paired slogans | Plain first-person copy based on the CV |
| “Let’s build something good” and ambiguous secondary CTA | “Email me” and “Download my CV,” describing their actual actions |
| A separate self-quotation/philosophy section | A short account of how Aviran uses and reviews AI-generated code within the about section |
| “Let’s make something good” in an oversized closing banner | A modest contact section with a direct email link |
| Repeated branded footer slogan and arrow-suffixed social links | Name in English and Hebrew, simple GitHub/LinkedIn/CV links |

### Visual structure — `index.html` and `style.css`

| Before | After |
| --- | --- |
| Decorative code tile, people icon, orbit lines, doodle arrow, and several sparkles | Actual portrait in the hero; one lilac arch preserves some of the references’ playfulness |
| Portrait as a tilted faux photograph in a second section | Unrotated portrait with a bilingual name caption; promoted from lazy-loading to high priority |
| Logo asterisks, numbered section eyebrows, decorative corner arrows | Removed; headings now carry the hierarchy without extra chrome |
| Keyword ticker and three oversized statistics | Removed; the user count is explained within the relevant Sofi work description |
| Three equally sized pastel service cards, each with an icon and skill pills | Actual Sofi and Beshutaf experience entries, with dates and responsibilities; earlier roles summarized underneath |
| Alternating promotional sections with repeated sales headings | Shorter introduction, motivation, experience, and contact structure |
| Cream/forest/lilac/peach used across numerous decorative surfaces | Cream and forest retained; lilac limited to portrait/selection, soft green groups experience; peach removed |
| Two similar sans-serif font families and excessive negative tracking | One family, DM Sans, with fewer weights and a restrained type scale |
| Tiny uppercase labels and 9–11px skill chips | Sentence-case copy and 13–16px supporting text; chips removed |
| Pill CTA, outlined nav CTA, arrows on most links | One modest rounded email button; ordinary navigation and underlined content links |
| Dense, minified CSS with rules for decorative components | Formatted CSS containing only the remaining layout and responsive styles |

## Boundaries

No invented clients, project screenshots, testimonials, hobbies, or outcomes were added. Career dates and metrics remain CV-sourced. The existing portrait-reuse and PDF-privacy notes in README still apply. No JavaScript, animation library, analytics, or build dependencies were introduced.

## Validation

- HTML nesting checked with Python’s standard-library HTMLParser.
- Desktop and mobile screenshots inspected. Browser full-page desktop capture produced repeated screenshot tiles; regular viewport captures and DOM section positions were used to distinguish this capture artifact from actual duplicate content.
- Browser assertions passed at 320, 390, 700, 768, 1024, and 1440px: no horizontal overflow, one h1, no skipped/empty headings, named links, valid local anchors, and a loaded portrait.
- Keyboard Tab exposed and focused the skip link; Enter activated it. Contact navigation reached `#contact`. The CV returned HTTP 200.
- Main and muted text colors passed WCAG AA on both cream and green backgrounds; the lowest tested ratio was 4.92:1.
