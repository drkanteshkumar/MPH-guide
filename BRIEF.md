# Brief for Claude Code: build the MPH Guide site

## Goal

Build a simple, clean static website from the content in the `content/` folder and publish it with GitHub Pages from this repository. This site is separate from my academic site (drkanteshkumar.github.io). Do not change that repository.

## Content (use the text exactly as written)

- `content/01-home-and-about.md` → Home page (title, short intro, buttons to each section) and an "About me" section
- `content/02-why-mph.md` → "Why an MPH" page
- `content/03-how-to-apply.md` → "How to apply" page
- `content/04-funding.md` → "Funding" page
- `content/05-ask-a-question.md` → "Ask a question" page

Do not rewrite, shorten or add to the text. Fix only obvious typos, and list any you fix.

## Links (already filled in the content files)

- MPH career options video: https://www.instagram.com/p/De0irNfuDEV/
- MPH application guide video: https://www.instagram.com/p/DeiOJWqBukD/
- Google Form: https://forms.gle/gnK3KozW5JasvmZ18

On the "Ask a question" page, embed the Google Form using this code, made responsive (width 100%, keep it readable on phones), and keep a plain "Open the form" button with the forms.gle link below it as a fallback:

```html
<iframe src="https://docs.google.com/forms/d/e/1FAIpQLScSbr1dwCrxj-l9MobFUtZKDFCStyVHsLtbCSZyYjYuCuA1_w/viewform?embedded=true" width="640" height="687" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
```

Show the Instagram video links as buttons.

## Structure and design

- Plain HTML and CSS, no build step and no frameworks, so GitHub Pages serves it directly. One HTML page per section, or one long page with anchor links: your choice, as long as the top navigation works.
- Top navigation on every page: Home · Why an MPH · How to apply · Funding · Ask a question
- Clean and readable: one simple font, generous spacing, max content width around 760px, one accent color (a deep red works well).
- Must look good on phones. Most visitors will come from Instagram.
- Tables must scroll sideways on small screens instead of breaking the layout.
- Checklist items in the Funding page can be plain bullets with a ☐ symbol (no interactive checkboxes needed).
- Footer on every page: "© Kantesh Kumar · Information checked October 2026. Always confirm details on official school websites." plus a link to my Instagram and my academic site (drkanteshkumar.github.io).
- Add a page title and meta description for each page, plus an Open Graph title, description and image so links shared on WhatsApp and Instagram show a nice preview.

## Publishing

1. Put the site files at the root of the repository (or in `/docs`, and set Pages to use that folder).
2. Enable GitHub Pages: repository Settings → Pages → Deploy from branch → `main`.
3. Give me the live link once it's up, and confirm every link and the form work on a phone-sized screen.

## Don'ts

- Don't add tracking, analytics, cookies or third-party scripts beyond the Google Form embed.
- Don't add content, testimonials or claims that aren't in the `content/` files.
- Don't touch my academic site repository.
