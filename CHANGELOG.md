# Changelog

All notable changes to Stux.Dev's `.github` organization repository are documented here.

Each release's sections come in this order: Added, Changed, Fixed, Removed, Security, Deprecated. This project adheres to [Date Versioning](https://datevers.ing) since v26.10.23 (`YY.MM.DD`, the UTC release date, with `-1`, `-2`… for later releases the same day); earlier releases used [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## v26.11.08

### Changed

- The Stux.Dev Status row says services are "checked regularly" instead of "every 5 minutes". GitHub runs the 5-minute schedule best-effort and often far less often, so the copy no longer promises 5 minutes; the status page shows the real check rhythm.

## v26.11.06-1

### Added

- A `test` branch. Work happens on `test`, and changes reach `main` only through a pull request from `test`, which needs CI to pass and is reviewed and merged by Leo; release commits and tags are made on `test` and go live when it's merged. CONTRIBUTING has a Branches section, its release steps end by pushing `test` and opening that pull request, and the README's Versioning section says so.
- `.github/workflows/ci.yml`, which runs `tests/version.sh` on pushes to `main` and `test` and on pull requests.

## v26.11.06

### Added

- The organisation profile lists **Stux.Dev Services** (services.stux.dev) and **Stux.Dev Status** (status.stux.dev), and a
  new **Our Templates** table lists Stux.Dev Soonpage, Maintenancepage, Servicepage and GitHub Pages Redirect, all by their
  full names. The intro links stux.dev and services.stux.dev.
- `CONTRIBUTING.md` has real code-style notes: leave the GitHup status table alone, use full service names, link only public
  repositories, and use light/dark logos.

### Changed

- The logos in `profile/README.md` and `README.md` follow GitHub's light or dark theme (`logo-light`/`logo-dark`), as do the
  footer icons. The footer's Stuxedo icon now comes from Stuxedo's media host instead of its GitHub avatar, and the footer
  says "Stux.Group Brand of Companies".
- Stuxs.Tools and Downl.one link their websites instead of their private repositories, which visitors couldn't open.
  AutoScroll links its site, with its repository alongside.
- `CONTRIBUTING.md` no longer mentions an `[Unreleased]` changelog section, which this repository doesn't use.
- This changelog's intro gives the house section order instead of citing Keep a Changelog, whose order differs. The README's
  copyright line names Stux.Group.

## v26.10.23

### Added

- `tests/version.sh`, which checks that `VERSION.md` is a valid Date Version, a real calendar date not in the future, and the same as the newest entry in this changelog

### Changed

- Switched from Semantic Versioning to [Date Versioning](https://datevers.ing): releases are numbered by their UTC release date as `YY.MM.DD`, with `-1`, `-2`… for later releases the same day. This release follows v1.3.1
- `commit.sh` and `commit.bat` refuse a `VERSION.md` that isn't a valid Date Version or is dated in the future (UTC), and warn when it's dated before today
- `README.md` and `CONTRIBUTING.md` describe Date Versioning and the release steps

## v1.3.1

### Changed

- Sm.lol's line in `profile/README.md` uses its new tagline, "The internet, but smol", matching the rebranded sm.lol homepage

## v1.3.0

### Added
- A **Service Status** section in `profile/README.md` with a live status badge and a status table for every Stux.Dev service (group, status, uptime and response time, linking to the new [status.stux.dev](https://status.stux.dev)), kept up to date hourly by the new `.github/workflows/status.yml` using GitHup's `readme` mode and the data in `StuxDev/Status`
- Stux.Dev Labs itself listed in "Our Labs Projects" in `profile/README.md`, linking to [labs.stux.dev](https://labs.stux.dev) (its repository is private), with the Stux.Dev Labs logo from `https://global.media.stux.dev/labs/logo.png` above the section

## v1.2.0

### Added
- New "Our Labs Projects" section in `profile/README.md`, linking to [Stux.Dev Labs](https://labs.stux.dev). AutoScroll moved here, matching its own "A Stux.Dev Labs Project" branding.

### Changed
- "Our Tools" split and renamed to "Our Services" in `profile/README.md`, now listing Stuxs.Tools, Downl.one, and Sm.lol.

## v1.1.0

### Added
- Sm.lol added to the "Our Tools" table in `profile/README.md`, as it is a Stux.Dev service. It has no public repository, so its entry links to [sm.lol](https://sm.lol) directly.

## v1.0.2

### Changed
- Renamed "Our Projects" to "Our Tools" in `profile/README.md` (and the matching "Explore our projects" call-to-action), matching the org's own tagline and mission copy, which both say "tools" throughout.

### Fixed
- The "Project" column of the tools table was rendering far too narrow for its contents, wrapping each entry's icon and link onto separate lines. Added a non-breaking space between icon and link text so each entry stays on one line.

## v1.0.1

### Added
- `README.md` gained the org slogan, "We build the tools we wished existed.", matching the `### *slogan*` heading pattern already used in Stux.Cloud's `.github` root README.

## v1.0.0

### Added
- Initial organization profile (`profile/README.md`)
- Organization-wide `README.md` and `CONTRIBUTING.md`
- `generateMetrics.yml` reusable workflow for the profile activity stats
- `VERSION.md` / `CHANGELOG.md` / `commit.sh` / `commit.bat` versioning setup
- "Our Projects" table in `profile/README.md`, linking out to Stuxs.Tools, Downl.one, and AutoScroll
