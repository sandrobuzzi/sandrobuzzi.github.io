This folder is reserved for future public-safe website content.

Rules:
- Keep only information here that you are comfortable publishing in the repository and on the website.
- During the draft phase, store working content in `private/content/` instead.
- Do not put private contact details, exact addresses, personal phone numbers, or unpublished material here.

Suggested workflow:
1. Store raw CV files and any sensitive source material in `private/`.
2. During drafting, store structured content in `private/content/`.
3. Only move sanitized summaries and structured data into `content/` when ready.
4. If you need a public CV later, generate it from a sanitized source instead of reusing the private one directly.

Practical split:
- `private/cv/cv.tex`: your full CV source with private details if needed.
- `private/cv/cv.pdf`: compiled output for private sharing.
- `private/content/*.yml`: draft website content derived from private material.
- `content/*.yml`: future sanitized website and public-profile data.

Recommendation:
Use `private/content/` as the canonical editable source while the site is private. If you later automate the site, scripts can read from those files locally and you can publish sanitized copies when ready.
