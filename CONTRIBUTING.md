# Contributing

Thank you for helping maintain the ActiveAdmin v4 Themes directory.

## Add or update a theme

1. Confirm that the theme has public source code and a recognized open-source
   license.
2. Verify the documented ActiveAdmin 4 version range.
3. Confirm that the installation path uses the ActiveAdmin 4 asset and styling
   model.
4. Add a concise entry to `README.md` with installation instructions,
   screenshots, and known limitations.
5. Run the local link check before opening a pull request.

We prefer evidence from the project's own README, test suite, demo application,
or a maintainer-confirmed compatibility statement. Do not copy third-party
theme source code or screenshots into this repository.

## Review standard

Maintainers check that entries are accurate, links resolve, images have useful
alternative text, and compatibility claims are specific. A theme may remain
outside the curated list when its AA4 support cannot be verified.

## Local checks

Run:

```bash
npx --yes markdown-link-check README.md
```

Pull requests run the same link check and Markdown linting in GitHub Actions.
