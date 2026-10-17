# Security policy

This is a static personal site served by GitHub Pages: no backend, no forms, no cookies, no third-party scripts.

If you spot a security issue, please use **Report a vulnerability** on this repository's Security tab rather than opening a public issue.

## Automated checks

| Check | Tool | When |
| --- | --- | --- |
| Secret scanning (full history) | Gitleaks | Every push, PR and weekly |
| Secret and misconfiguration scan | Trivy, results in the Security tab | Every push, PR and weekly |
| Action version updates | Dependabot | Weekly |
