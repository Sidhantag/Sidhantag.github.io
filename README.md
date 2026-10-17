# sidhantag.github.io

![Site quality](https://github.com/Sidhantag/sidhantag.github.io/actions/workflows/site-quality.yml/badge.svg)
![Security](https://github.com/Sidhantag/sidhantag.github.io/actions/workflows/security.yml/badge.svg)

Personal portfolio of **Sidhant Ghuge**, Quality Engineering & DevSecOps. Live at **https://sidhantag.github.io**.

## How it's built

- React app built with Vite into a single self-contained `index.html` (scripts, styles and images inlined), so the page loads with one request and depends on no CDN or third-party script.
- Hosted on GitHub Pages from the `main` branch.

## Quality gates

I treat this site like any production release:

| Gate | Tool | Fails the build when |
| --- | --- | --- |
| Broken links | Lychee | Any outbound link stops resolving (also runs weekly) |
| Accessibility | Lighthouse CI | Score below 90 |
| SEO | Lighthouse CI | Score below 90 |
| Performance, best practices | Lighthouse CI | Warns below 80 / 90 |
| Secrets | Gitleaks + Trivy | A credential is committed anywhere in history |
| Misconfiguration | Trivy | A risky config is found (results in the Security tab) |

Lighthouse reports from each run are uploaded as build artifacts with a public report link in the job log.
