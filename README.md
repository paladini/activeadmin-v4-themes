# ActiveAdmin v4 Themes

[![Link checks](https://github.com/paladini/activeadmin-v4-themes/actions/workflows/ci.yml/badge.svg)](https://github.com/paladini/activeadmin-v4-themes/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An awesome-style directory of themes built for ActiveAdmin 4 and its new
Tailwind CSS-based interface.

> **Scope:** This list includes themes with documented, verifiable support for
> ActiveAdmin 4. Legacy ActiveAdmin 3 and SCSS themes do not belong in the main
> list.

## Contents

- [Curated themes](#curated-themes)
- [What counts as ActiveAdmin 4 support?](#what-counts-as-activeadmin-4-support)
- [Excluded and pending projects](#excluded-and-pending-projects)
- [How to submit a theme](#how-to-submit-a-theme)

## Curated themes

### Active Admin Claude Theme

[![Login screen](https://raw.githubusercontent.com/paladini/activeadmin-claude-theme/main/docs/images/login.png)](https://github.com/paladini/activeadmin-claude-theme)

[![Dashboard](https://raw.githubusercontent.com/paladini/activeadmin-claude-theme/main/docs/images/dashboard.png)](https://github.com/paladini/activeadmin-claude-theme)

[![Admin users](https://raw.githubusercontent.com/paladini/activeadmin-claude-theme/main/docs/images/admin_users.png)](https://github.com/paladini/activeadmin-claude-theme)

[![Dark mode](https://raw.githubusercontent.com/paladini/activeadmin-claude-theme/main/docs/images/dashboard_dark.png)](https://github.com/paladini/activeadmin-claude-theme)

A warm, editorial theme inspired by Claude and Anthropic aesthetics. It
recolors ActiveAdmin 4 through Tailwind v4 theme tokens and CSS variables,
while preserving the built-in dark-mode toggle, mobile drawer, and Flowbite
hooks.

| Field | Details |
| --- | --- |
| Project | [paladini/activeadmin-claude-theme](https://github.com/paladini/activeadmin-claude-theme) |
| License | MIT |
| ActiveAdmin | `4.0.0.beta22+` |
| Styling | Tailwind CSS v4 |
| Rails integration | Rails Engine gem with an install generator |
| Status | AA4 verified |

#### Install

Add the gem to your Rails application's `Gemfile`:

```ruby
gem "activeadmin-claude-theme"
```

Then install the gem and run its generator:

```bash
bundle install
rails generate activeadmin_claude_theme:install
npm run build:css
```

Your application must already use ActiveAdmin 4 with Tailwind v4 assets. See
the [theme installation guide](https://github.com/paladini/activeadmin-claude-theme#installation)
for the required ActiveAdmin, `cssbundling-rails`, and `importmap-rails`
setup.

#### Known limitations

- The theme requires ActiveAdmin `4.0.0.beta22` or newer.
- It is not a drop-in replacement for legacy Sprockets or SCSS themes.
- Anthropic and Claude are referenced for design inspiration only; the project
  is not affiliated with or endorsed by Anthropic.

## What counts as ActiveAdmin 4 support?

A project qualifies for the curated list when its documentation or tests
provide enough evidence that it works with the ActiveAdmin 4 architecture:

- It names an ActiveAdmin 4 version or range, ideally including the latest
  beta.
- Its installation instructions use the ActiveAdmin 4 asset pipeline and
  styling model, rather than only `active_admin/base` SCSS imports.
- Its screenshots or demo show the theme running in an ActiveAdmin 4 app.
- Its license and source repository are publicly available.

ActiveAdmin 4 is still released as a beta series. The latest version checked
for this list is `4.0.0.beta22`. Confirm the upstream compatibility range before
installing a theme in production.

## Excluded and pending projects

The following projects were found during the initial survey but are not listed
as ActiveAdmin 4 themes because their current documentation does not verify
compatibility with the AA4 Tailwind architecture:

- [Arctic Admin](https://github.com/cprodhomme/arctic_admin) — SCSS-based
  integration documented for the classic asset pipeline.
- [ActiveAdminTheme](https://github.com/activeadmin-plugins/active_admin_theme)
  — legacy SCSS theme with ActiveAdmin 3-era installation instructions.
- [Light Admin](https://github.com/CapSens/light_admin) — classic SCSS theme;
  AA4 compatibility is not documented.
- [ActiveAdmin Blaze Theme](https://github.com/blocknotes/activeadmin_blaze_theme)
  — Blaze CSS and legacy ActiveAdmin asset integration.
- [ActiveAdmin AAA Theme](https://github.com/paladini/activeadmin-aaa-theme)
  — modern visual design, but its current documentation targets ActiveAdmin
  3+ and SCSS rather than verified AA4 support.
- [ActiveAdmin Prism](https://github.com/ramlaxmanyadav/active_admin_prism)
  — promising candidate that declares `ActiveAdmin >= 3.0`, but still needs
  an AA4/Tailwind compatibility demonstration.

These projects may become eligible when their maintainers document and verify
ActiveAdmin 4 support. They are not quality judgments.

## How to submit a theme

Open an issue using the [new theme template](https://github.com/paladini/activeadmin-v4-themes/issues/new?template=new-theme.yml),
or submit a pull request with the following information:

- project name and canonical repository link;
- license and package or gem name;
- supported ActiveAdmin versions;
- styling and asset pipeline requirements;
- installation commands;
- screenshots or a public demo running ActiveAdmin 4;
- known limitations and maintenance status.

Please keep entries factual and link to the original project. This repository
curates and documents themes; it does not redistribute third-party code.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for the review and verification
workflow. The list was last curated on **July 16, 2026**.

## License

The directory content is available under the [MIT License](LICENSE). Each
listed project keeps its own license and ownership.
