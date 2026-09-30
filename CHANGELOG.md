# Changelog

All notable changes to Stux.Dev's `.github` organization repository are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

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
