# CLAUDE.md

- **This is a repository template** - Keep code minimal and generic — do not add real Polarion integration logic or domain-specific functionality.
- **Version `0.0.0` in `pyproject.toml` is intentional** — the CI/CD pipeline (Release Please) sets the real version from git tags. Never change it.
- **SBB GitHub Actions workflows are pinned to `@main`, not hash-pinned** — `SchweizerischeBundesbahnen/*` reusable workflows intentionally use branch refs. This is enforced by `zizmor.yml`. Do not convert these to commit hash pins.
