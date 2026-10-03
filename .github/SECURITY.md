# Security Policy

## Reporting a vulnerability

Do not report vulnerabilities through public GitHub issues, pull requests, or Discord.

Use **Report a vulnerability** on the affected repository's **Security** tab when private vulnerability reporting is enabled. For the apps:

- [Report a Thaw vulnerability](https://github.com/thaw-app/Thaw/security/advisories/new).
- [Report a Floe vulnerability](https://github.com/thaw-app/Floe/security/advisories/new).

If private reporting is unavailable, contact the maintainer privately through the contact method on their [GitHub profile](https://github.com/diazdesandi). Do not publish exploit details while looking for a reporting channel.

Include the affected repository, version or commit, operating system, reproduction steps, and potential impact. Remove credentials and unrelated personal data from logs and attachments.

## Supported versions and scope

Support windows and security guarantees are project-specific. Read the repository's security notes:

- [Thaw security notes](https://github.com/thaw-app/Thaw/blob/development/docs/SECURITY_NOTES.md).
- [Floe security notes](https://github.com/thaw-app/Floe/blob/main/docs/SECURITY_NOTES.md).
- Other repositories: check their README, release documentation, and any project-specific security notes.

These organization defaults do not imply that every project has signed releases, sandboxing, an update feed, or the same support window.

## Coordinated disclosure

Maintainers acknowledge and triage reports, investigate affected versions, and prepare fixes privately where needed. Response times depend on the project, severity, and whether a third-party or operating-system fix is required. Project-specific response targets are in the security notes.

Coordinate public disclosure with maintainers so users can obtain a fix or mitigation first. Maintainers publish confirmed vulnerabilities through GitHub Security Advisories and credit reporters unless they request anonymity. Please keep reports confidential until the agreed disclosure date.

## Dependency findings

Do not bypass required dependency checks. Prefer upgrading or removing a vulnerable dependency. If a finding is not exploitable or must be temporarily accepted, document the reason and an expiry in the project's suppression file and obtain maintainer review. Project security notes define scanned artifacts, thresholds, and suppression locations.
