# TrustAI BrandGuard

An explainable AI tool for brand governance. It reviews content before it is published, checks it against approved brand guidelines and facts, explains each issue with its source, and leaves the final decision to people.

> **Status:** Round 1, plan stage. This repository contains the marketing site and an interactive demo. The full review engine, source library and approval workflow are planned and not yet built.

## Features

**In this repository (demo)**
- Marketing site with product overview, workflow, status and contact sections.
- Live check: type or paste ad copy and see flagged issues and a suggested revision. It uses a few fixed demo rules and a sample product sheet.
- Contact form with local validation. It does not send requests yet.

**Planned**
- Source library for guidelines, approved facts and reusable assets.
- Fact and promotional-claim checking against approved sources.
- Tone, terminology and messaging consistency checks.
- Visual identity and accessibility checks.
- Explainable findings with suggested corrections.
- Comments, approvals, version history and audit trail.

## How it is meant to work

1. **Import**: add brand guidelines, approved facts, terminology and assets.
2. **Upload**: submit text, images, advertisements or documents.
3. **Analyse**: check tone, claims, facts, visuals, messaging and accessibility.
4. **Improve**: explain each issue and suggest a correction with its reference.
5. **Approve**: a human reviewer approves the content or requests changes.

## Principles

- Every finding includes its reason and source.
- Unsupported claims are flagged for review, not automatically declared false.
- Publication decisions stay with authorised people.
- External AI use is disclosed. Data sent to an external AI service may be transmitted depending on the provider and configuration.

## Getting started

No build step is needed.

```bash
git clone https://github.com/harshareddy1829/trustai-brandguard.git
cd trustai-brandguard
open index.html        # macOS; on Windows, double-click the file; on Linux, xdg-open index.html
```

The page loads two fonts from Google Fonts, so it needs an internet connection for the intended typography. It still works offline with fallback fonts.

## Project structure

```
.
├── index.html   # Full site: markup, styles and the demo script (single file)
├── README.md
└── .gitignore
```

## Deployment

The site is a single static file, so it can be hosted on GitHub Pages:

1. Push the repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then save.

The site will be available at `https://harshareddy1829.github.io/trustai-brandguard/`.

## Roadmap

- [ ] Working prototype of the review engine
- [ ] Source library and guideline import
- [ ] User research: interviews, survey and testing with sample guidelines
- [ ] Evaluation against a test set of known issues
- [ ] Contact form connected to a real backend

## Evaluation

These metrics will be measured during testing. No results exist yet.

- Known issues correctly identified in a test set
- Time required to review and correct sample content
- Reviewer rating of whether findings are clear and useful

## Limitations

- The live demo is not the review engine. It uses fixed rules, so it will miss issues and can flag correct content.
- Examples and the product sheet on the site are fictional.
- The contact form does not send any data.

## License

To be decided by the project owners.
