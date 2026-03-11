# AGENTS.md

## Testing Requirements
All changes must pass `python test_environment.py` before committing.
Any code added to `src/` must have a corresponding test in `tests/`
that passes before the change is pushed.

## Secrets Policy
Do not include API keys, passwords, tokens, or raw hospital data in prompts.
Never commit `.env`, `*.key`, `*.pem`, raw CSV files, or any file that
contains credentials or sensitive project data.

## Scope Boundaries
Agents may edit `README.md`, `CHANGELOG.md`, `AGENTS.md`, `src/`,
`notebooks/`, and `tests/` when needed.
Do not modify `requirements.txt` without human review.
Do not modify `setup.sh` without running it locally after the change.
Do not modify `.gitignore` unless you verify that source files are not excluded.
Do not commit files inside `data/raw/` or the `.venv/` directory.

## Reproducibility Standard
All AI-assisted changes must be tested locally before commit or push.
A change is only considered done when it runs locally and produces the
expected result. AI-generated output must be reviewed by a human before submission.