# TODO

## In Progress

- [ ] Populate `containers/README.md` with DockerHub image links (when published)
- [ ] Fill in `PROTOCOLS.md` parameter table (resolution, TR/TE, acceleration, operating mode per sequence)

## Planned

- [ ] Fix critical script bugs flagged in `REVIEW.md` §3/§5
- [ ] Add `requirements.txt` / `environment.yml` for Python scripts
- [ ] Document minimum FSL version requirement in `scripts/README.md`
- [ ] CI: shell script linting with `shellcheck`
- [ ] CI: Python linting with `ruff`
- [ ] Add `docs/` guides: how-to-run, FAQ, troubleshooting

## Needs Expert Sign-Off

See `REVIEW.md` §6 for full details.

- [ ] Confirm operating mode (1st-level / 2nd-level) for each protocol
- [ ] Verify XA30 feature compatibility for all sequences
- [ ] Validate SAR limits per protocol
- [ ] Clarify delta TE choice for ME-BOLD (REVIEW.md §7, Q1)
- [ ] Confirm phase unwrapping method (REVIEW.md §7, Q2)
