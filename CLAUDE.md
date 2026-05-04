# Expense Tracker

## Windows Compatibility
- Avoid Unicode box-drawing characters (─, │, ┌, etc.) and special symbols (€, £, etc.) in logging/print output as they break Windows cp1252 encoding.
- Use ASCII alternatives or explicitly set UTF-8 encoding with `sys.stdout.reconfigure(encoding='utf-8')` or configure logging handlers with `encoding='utf-8'`.

## Git Operations
- Never assume the default branch is `main` — always run `git branch --show-current` or `git symbolic-ref HEAD` first before pushing or referencing branches.
- This machine uses multiple GitHub accounts (personal + work) configured via SSH host aliases; use the appropriate remote URL (e.g., `git@github-personal:user/repo.git`) rather than HTTPS.
