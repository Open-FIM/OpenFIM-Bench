# Contributing to OpenFIM-Bench

Thanks for your interest in contributing to OpenFIM-Bench — a community effort
to build population-grounded, expert-governed benchmarks for evaluating
Food-is-Medicine (FIM) AI. Contributions from nutrition/public-health experts,
clinicians, and AI/ML practitioners are all welcome.

## Ways to contribute

- **Benchmark cases**: proposing or reviewing structured person-level
  nutrition cases (from NHANES, MIMIC, or synthetic sources)
- **Expert assessment**: RDN or clinical review of cases, including flagging
  disagreement, acceptable variation, or safety boundaries
- **Evaluation methodology**: scoring rubrics, agreement metrics, or task
  definitions (e.g., condition-to-food recommendation, cultural cuisine
  adaptation, budget/access-constrained planning, drug-nutrient interaction
  flagging, plan communication quality)
- **Tooling**: data-processing scripts, synthetic-data generation, benchmark
  harnesses, documentation
- **Bug reports and issues**: use GitHub Issues for anything you find broken
  or unclear

## Before you start

1. Check open [Issues](../../issues) and [Pull Requests](../../pulls) to
   avoid duplicate work.
2. For substantial changes (new task types, changes to benchmark
   methodology, or new data sources), please open an issue first to discuss
   the approach before submitting a PR.
3. By submitting a contribution, you agree it is licensed under the
   project's [Apache License 2.0](LICENSE) (see "Developer Certificate of
   Origin" below).

## Data handling — please read

This project works with sensitive population health data. Contributors
must:

- **Never commit raw, identifiable, or restricted-access data** (e.g., raw
  NHANES public-use files large enough to redistribute wholesale, or any
  MIMIC-derived data, which requires a signed PhysioNet Data Use Agreement
  and credentialed access and may not be redistributed here).
- Prefer derived, de-identified, or synthetic case representations, and
  document the provenance and transformation pipeline for any dataset you
  add or modify.
- Flag any uncertainty about data sensitivity in your PR description so
  maintainers can review before merge.

## Submitting a pull request

1. Fork the repository and create a branch from `main`.
2. Make your changes, with clear, focused commits.
3. Include or update documentation (README, data-source notes) relevant to
   your change.
4. Reference any related issue in your PR description.
5. A maintainer will review; benchmark-content PRs (new cases, scoring
   changes) may also need review from a qualified RDN or clinical
   contributor before merge.

## Developer Certificate of Origin (DCO)

By contributing, you certify that you wrote the contribution yourself, or
otherwise have the right to submit it under the project's open-source
license, per the [Developer Certificate of Origin](https://developercertificate.org/).
Please sign off your commits:

```
git commit -s -m "Your commit message"
```

## Code of Conduct

This project follows the [Code of Conduct](CODE_OF_CONDUCT.md). Please read
it before participating.

## Questions

Open a [Discussion](../../discussions) or [Issue](../../issues) — we're
happy to help newcomers get oriented, especially nutrition/clinical experts
who may be new to open-source workflows.
