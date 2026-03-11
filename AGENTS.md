# AGENTS.md

## Testing Requirements
All changes must pass `python test_environment.py` before committing.
If new code is added later, it should also be tested locally before pushing.
The environment must stay reproducible with `requirements.txt` and `setup.sh`.

## Secrets Policy
Do not include API keys, passwords, tokens, or personal data in prompts or commits.
Never commit `.env`, `*.key`, `*.pem`, or raw data files.
Sensitive information must stay outside the repository.

## Scope Boundaries
Agents may edit `README.md`, `requirements.txt`, `.gitignore`, `setup.sh`, and `AGENTS.md` in this project.
Do not modify `test_environment.py` or files inside `tests/` because they are used for validation.
Any major dependency changes should be reviewed carefully before committing.

## Reproducibility Standard
All AI-assisted changes must be verified locally before they are committed or pushed.
A change is only considered complete if the environment runs successfully and `python test_environment.py` prints `Environment OK`.
“The AI generated it” is not enough without local verification.