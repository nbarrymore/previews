# previews

Shareable, co-author-facing review materials, served as live web pages via
GitHub Pages. Use it to hand collaborators a working link to something (an
interactive survey draft, a figure, an explainer) without emailing files or
fighting local-file security blocks.

**Live site:** https://nbarrymore.github.io/previews/

## Standing rule: everything here is PUBLIC by URL

This repo is public and the pages are reachable by anyone who has the link.
Only put material here that is safe to be public:

- **No PII, no raw data, no credentials.**
- **No embargoed or scoop-sensitive results.** If a preview shouldn't be
  publicly reachable, share it a different way (a login-gated host).
- Prefer **self-contained** pages (all CSS/JS/images inline) so a single
  `index.html` renders anywhere with no external dependencies.

## Layout

```
<project>/<thing>/index.html   ->  https://nbarrymore.github.io/previews/<project>/<thing>/
```

One folder per project, one subfolder per preview. Example:

- `ambition/study2/` — Study 2 human task-typing survey draft (interactive).

## Publishing a new preview

1. Build the self-contained HTML in the project repo (its own source is the
   source of truth).
2. Copy it here as `<project>/<thing>/index.html`.
3. Commit and push. GitHub Pages redeploys automatically (a minute or two).
