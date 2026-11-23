# AGENTS.md

## Commands
- Sync env: `uv sync --locked`
- Run anything: `uv run <cmd>` (never bare python/pip)
- Tests: `uv run pytest`
- Lint: `uv run ruff check .`
- Format: `uv run ruff format --check .`
- Before finishing any task: run the lint + format + tests above and report results.

## Layout
- Source in `src/`
- Tests in `tests/` (mirror package structure)
- Treat `uv.lock` as generated — update only via `uv`

## Rules
- Use type hints on public functions.
- Prefer small, focused changes.
- Do not add production dependencies without asking.
- Never edit `.env*` or commit secrets.
- Keep changes limited to the requested task.
- Do not over-engineer the code.
- Do not be overly defensive in coding.
