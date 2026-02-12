# Contributing

Thanks for your interest in contributing to **Tray Mode Drift Detector**!

## Quick start (dev)

1. Fork the repo and clone your fork.
2. Create a feature branch:
   - `git checkout -b feat/<short-name>`
3. Install dependencies (choose one):
   - **pip**: `python -m pip install -r requirements.txt`
   - **poetry** (if used): `poetry install`
4. Run checks locally (recommended):
   - `python -m compileall .`
   - `python -m pip install ruff`
   - `ruff check .`
5. Open a pull request with a clear description of:
   - What problem you’re solving
   - What you changed
   - How you tested it

## Contribution guidelines

- Keep changes focused and small when possible.
- Prefer clear, explicit names over clever ones.
- Add or update docs when behavior changes.
- If you add functionality, add at least a minimal test or example.

## Commit message style

Use a simple convention:

- `docs: ...`
- `fix: ...`
- `feat: ...`
- `chore: ...`

## Reporting issues

If you found a bug or gap in documentation, please open an issue and include:

- What you expected to happen
- What actually happened
- Steps to reproduce (copy/paste friendly)
- Any relevant logs or files (redact secrets)
