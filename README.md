<p align="center">
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.dev/logo-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.dev/logo-dark.png"><img src="https://global.media.stux.dev/logo-dark.png" height="100" alt="Stux.Dev Logo"></picture>
</p>

# .github

### *We build the tools we wished existed.*

The central repository for the Stux.Dev GitHub organization configuration and profile settings.

## Overview

This repository contains the organization-wide configuration files for the Stux.Dev GitHub profile, including community health files and the org's public profile page.

## What's Included

- **Profile** — the public org profile shown at [github.com/StuxDev](https://github.com/StuxDev) (`profile/README.md`)
- **Community Files** — contributing guidelines and other org-wide defaults
- **Service Status table** — `.github/workflows/status.yml` refreshes the table between the `<!-- githup:start -->` / `<!-- githup:end -->` markers in `profile/README.md` every hour with [GitHup](https://githup.stux.group)'s `readme` mode, from the data in [StuxDev/Status](https://github.com/StuxDev/Status) ([status.stux.dev](https://status.stux.dev)); don't edit inside the markers
- **Metrics** — `.github/workflows/generateMetrics.yml` renders the "Our Activity" image

## How It Works

GitHub automatically applies files from this `.github` repository to all public repositories in the organization (when a specific repository doesn't have its own version), and renders `profile/README.md` as the org's public profile page.

## Getting Started

```bash
git clone https://github.com/StuxDev/.github.git
cd .github
```

## Development

See [CONTRIBUTING.md](CONTRIBUTING.md) for the development workflow and release process.

## Versioning

This project uses [Date Versioning](https://datevers.ing): each release is numbered by its UTC release date as `YY.MM.DD` (for example `26.10.23`), with `-1`, `-2`… for later releases the same day. See [CHANGELOG.md](CHANGELOG.md) for what changed in each release.

## Copyright

Copyright © 2026 Stux.Group. All rights reserved. Stux.Dev is operated by **Stux Group Ltd**, a company registered in England and Wales (company no. 13160574).

---

*Built & Maintained by <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.dev/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.dev/icon-dark.png"><img src="https://global.media.stux.dev/icon-dark.png" height="14" alt="Stux.Dev" valign="middle"></picture> [Stux.Dev](https://github.com/StuxDev), Hosted by <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stuxedo.com/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stuxedo.com/icon-dark.png"><img src="https://global.media.stuxedo.com/icon-dark.png" height="14" alt="Stuxedo" valign="middle"></picture> [Stuxedo](https://stuxedo.com).  
Stux.Dev is a part of the <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.group/icon-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.group/icon-dark.png"><img src="https://global.media.stux.group/icon-dark.png" height="14" alt="Stux.Group" valign="middle"></picture> Stux.Group Brand of Companies.*
