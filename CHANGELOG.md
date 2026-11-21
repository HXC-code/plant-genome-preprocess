# Changelog

## 3.4.4 — 2026-11-21

- Species analysis codes: genus initial plus two specific-epithet letters, widening to three/four or more letters on collision, with a numeric suffix only as a last resort. Table rows keep their published codes; new species are derived from the Latin name and avoid every existing code.
- Documentation: README and QUICKSTART rewritten around the actual job — preprocessing the user's own raw downloads into WGDI inputs. Input-format coverage now reflects content-based detection, compression magic and `A|B` candidate routing. Install paths, Python requirement (>= 3.11), smoke-test paths and skill-package location corrected.
- Packaging: MIT `LICENSE` added to both repositories.
- Engineering: `pytest` (151 tests), `ruff` and `mypy` all pass. GitHub Actions added for push/PR. `tests/conftest.py` now redirects pytest when the default temp root is unwritable or too deep. `sync_skill_package.py` gained `--pipeline-target` to check/sync the released `pipeline/` mirror.
- Minor: removed an unused `csv` import in `naming_audit.py` and fixed three type errors in `artifact_migration.py` / `cli.py`.
