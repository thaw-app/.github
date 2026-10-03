# Contributing to Thaw/Floe

Bug reports, code, documentation, and translations are welcome. Follow the [Code of Conduct](https://github.com/thaw-app/.github/blob/main/.github/CODE_OF_CONDUCT.md).

## Getting started

Read the repository's README and `docs/DEVELOPMENT.md` for build commands and tests. Fork the repository and create a branch for your change. Target the `development` branch when present; otherwise target the default branch, unless a maintainer asks otherwise.

If translations are managed through Crowdin, contribute through the project's configured Crowdin project rather than opening translation pull requests.

Search existing issues before reporting a bug. Include enough detail to reproduce it and use the repository's issue template. Report vulnerabilities privately using the [Security Policy](https://github.com/thaw-app/.github/blob/main/.github/SECURITY.md), not public issues or Discord.

## Pull requests

Discuss features, substantial refactors, and sensitive changes in an issue before implementation. Keep pull requests focused; aim for no more than 500 changed lines and 20 files. Explain larger changes and link the agreed scope.

Use Conventional Commit titles, such as `fix(runtime): handle missing preferences` or `docs: clarify build requirements`. Fill in the repository's pull request template, link the relevant issue, and state which checks you ran. Leave unchecked items unchecked when they do not apply or were not run.

Add automated tests for new behavior and regression tests for bug fixes when practical. Update affected documentation. Required checks must pass before merge. Address review findings unless a maintainer explicitly accepts the risk or marks a finding as not applicable. Dependency suppressions need a documented reason and an expiry; follow the [Security Policy](https://github.com/thaw-app/.github/blob/main/.github/SECURITY.md#dependency-findings).

Maintainers may close pull requests with failing checks left unaddressed, ignored feedback, missing required tests or documentation, or unreviewed generated content. If requested changes receive no meaningful follow-up, open a new pull request later that addresses the feedback.

## Developer Certificate of Origin

Sign off your commits to certify that you have the right to submit the work under the repository's license, using the [Developer Certificate of Origin v1.1](https://developercertificate.org/):

```sh
git commit -s -m "fix: describe the change"
```

Use your real name and an email matching the commit author. This adds a `Signed-off-by` trailer; it is not a cryptographic signature, a CLA, or a transfer of copyright. Automated enforcement and bot exemptions are defined by the repository's PR Metadata workflow; do not assume every repository has a DCO check.

## AI-assisted contributions

AI-assisted work has the same review requirements as other contributions. You are responsible for the submitted code, its provenance, tests, and license compatibility. You must understand the change and be able to explain it in review.

Use tools whose terms permit contributing their output under the repository's license. Do not submit proprietary or restricted third-party code as your own. Review generated output before opening the pull request.

## Questions

Questions are welcome on the [community Discord](https://discord.gg/KDfWjWDnR4). Keep bug reports and project decisions in GitHub issues and pull requests so others can find them.
