# Contributing

Thanks for your interest in contributing to this project.

## Development Workflow

1. Create a feature branch off `main`.
2. Make focused, well-described commits.
3. Describe your changes in a new release entry in `CHANGELOG.md` (see [Versioning](#versioning)).
4. Open a pull request against `main`.

## Code Style

- Don't edit the Service Status table between `<!-- githup:start -->` and `<!-- githup:end -->` in `profile/README.md`: `.github/workflows/status.yml` rewrites it every hour from [StuxDev/Status](https://github.com/StuxDev/Status).
- Use each service's full name ("Stux.Dev Status", not "Status"), matching its card on [services.stux.dev](https://services.stux.dev). When a service is added, renamed or retired there, update the profile tables to match.
- Only link a repository if it's public. Link a private service's website instead.
- Logos and icons come from the brands' media hosts (`global.media.stux.dev` and so on), as light/dark `<picture>` elements, so they follow GitHub's theme.

## Versioning

This project uses [Date Versioning](https://datevers.ing). To release:

1. Add a `## vYY.MM.DD` entry at the top of `CHANGELOG.md`, with its sections in this order: Added, Changed, Fixed, Removed, Security, Deprecated.
2. Set `VERSION.md` to the same bare version (no `v`): today's **UTC** date as `YY.MM.DD`, or `YY.MM.DD-1`, `-2`… for later releases the same UTC day. Never a future date. Use UTC, not local time: just after midnight in the UK it is still the previous day in UTC.
3. Run `bash tests/version.sh`.
4. Run `./commit.sh` (or `commit.bat` on Windows). It checks the version, commits and tags `vYY.MM.DD`, and never pushes.
