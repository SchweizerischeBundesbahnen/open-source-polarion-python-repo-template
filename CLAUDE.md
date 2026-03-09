# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Python repository template for open-source Polarion projects by SBB (Schweizerische Bundesbahnen). It serves as a standardized template for creating Python packages that integrate with Polarion ALM systems.

**Key Requirements:**
- Python 3.13+ (version pinned in `.tool-versions`)
- uv for dependency management
- All contributors must have an active Polarion license
- Follows Conventional Commits for commit messages
- Uses DCO (Developer Certificate of Origin) - all commits must be signed

## Development Commands

### Setup
```bash
# Install dependencies
uv sync --all-groups
```

### Testing and Quality Assurance
```bash
# Run all checks and tests via tox
uv run tox

# Run specific tox environments
uv run tox -e ruff    # Ruff linting and formatting only
uv run tox -e mypy    # Type checking only
uv run tox -e test    # Tests with coverage only

# Individual commands
uv run pytest tests/ --junitxml="junittest.xml"
uv run coverage run -m pytest tests/
uv run coverage report -m --fail-under 90
uv run coverage xml
```

### Code Formatting and Linting
```bash
# Format code
uv run ruff format

# Check and fix linting issues
uv run ruff check

# Type checking
uv run mypy .
```

### Build
```bash
# Build the package
uv build
```

## Project Structure

- `open_source_polarion_python_repo_template/` - Main package directory
  - `__init__.py` - Package initialization (currently empty)
  - `dummy.py` - Template/example module
- `tests/` - Test directory following pytest conventions
- `.tool-versions` - Python version pin (used by uv and CI)
- `CODING_STANDARDS.md` - Detailed coding standards (covers Python, Java, Docker)
- `CONTRIBUTING.md` - Contribution guidelines with DCO requirements

## Code Quality Standards

### Python Standards
- Follows PEP 8 via ruff with extended rules
- Line length: 240 characters
- Uses mypy for type checking with strict settings (`disallow_untyped_defs = true`)
- Minimum test coverage: 90%
- Tests exclude assert rule violations (S101 ignored in tests)

### Commit Standards
- Must follow Conventional Commits format
- All commits must be GPG signed (configured via global git config)
- Enforced via commitizen in CI/CD

## CI/CD Pipeline

The repository uses GitHub Actions with:
- **PR Checks**: Validates conventional commit messages
- **Build & Release**: Runs tox, SonarCloud analysis, and release-please
- **Quality Gates**: SonarCloud integration with quality metrics
- **Automated Releases**: Uses release-please for Python packages

## Architecture Notes

This is a template repository with minimal code structure:
- Simple package layout with one dummy module
- Standard Python testing setup with pytest
- uv-based dependency management with `hatchling` as build backend
- Comprehensive linting and formatting pipeline (ruff, mypy, separate tox envs)
- SBB-specific requirements (Polarion license, DCO signing)

The template is designed to be cloned and modified for actual Polarion integration projects.
