# CLAUDE.md

- Use `uv` for all Python tooling (`uv run tox`, `uv run pytest`, `uv sync`, `uv build`) — never `pip`, `python -m pip`, or bare tool invocations.
- Always use `uv sync --locked` — verifies lockfile is consistent with `pyproject.toml`; never `--frozen`.
- Signed commits are required (GPG enforced via git config conditional includes).
- This is a repository template. Keep code minimal and generic — do not add real Polarion integration logic or domain-specific functionality.
- Line length is 240 characters (configured in ruff) — do not reformat to shorter lengths.
- GitHub Actions workflows from `SchweizerischeBundesbahnen/*` are intentionally pinned to `@main`, not hash-pinned. This is enforced by `zizmor.yml`. Do not change these to hash pins.
