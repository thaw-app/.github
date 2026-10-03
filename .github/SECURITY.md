# Thaw/Floe Security Policy

## Reporting a vulnerability

Do not report vulnerabilities through public GitHub issues, pull requests, or Discord.

Use **Report a vulnerability** on the affected repository's **Security** tab when private vulnerability reporting is enabled:

- [Report a Thaw vulnerability](https://github.com/thaw-app/Thaw/security/advisories/new).
- [Report a Floe vulnerability](https://github.com/thaw-app/Floe/security/advisories/new).

If private reporting is unavailable, contact the maintainer privately through the contact method on their [GitHub profile](https://github.com/diazdesandi). Do not publish exploit details while looking for a reporting channel.

Include the affected repository, version or commit, macOS version, reproduction steps, and potential impact. Remove credentials and unrelated personal data from logs and attachments.

## Supported versions

Security fixes target the latest stable release. Older releases are not supported. For projects without a stable release, reproduce on the current default branch. Alpha and beta releases receive best-effort support.

## Scope

Report privilege escalation, unauthorized access to application-managed data, arbitrary code execution through crafted input, permission bypasses, and compromised or forgeable release or update paths attributable to Thaw/Floe.

Crashes without an exploit path, physical access to an unlocked Mac, social engineering, and flaws solely in third-party components are generally out of scope. Report third-party vulnerabilities to their maintainers unless Thaw/Floe needs a mitigation.

Running a third-party extension or script is not a sandbox boundary. Only run code you trust; it may access files and the network under your user account. This policy does not promise protection against attackers who already control your Mac session or hold the same permissions.

## Coordinated disclosure

Maintainers aim to acknowledge reports within 48 hours (best effort), investigate affected versions, and prepare fixes privately where needed. Fix timelines depend on severity, complexity, and whether a third-party or operating-system fix is required.

Coordinate public disclosure with maintainers so users can obtain a fix or mitigation first. Maintainers publish confirmed vulnerabilities through GitHub Security Advisories, assign CVEs when appropriate, and credit reporters unless they request anonymity. Please keep reports confidential until the agreed disclosure date.

## Dependency findings

Repositories with Dependency SCA checks must resolve every unsuppressed finding before merge, regardless of severity. Prefer upgrading or removing the affected dependency. Dependabot updates must pass the same checks.

If a finding is not exploitable or must be temporarily accepted, add a suppression with `reason` and `ignoreUntil` (YYYY-MM-DD) and obtain maintainer review. The reason must explain why the finding is acceptable for the application; the expiry ensures it is revisited. Suppressions live in `osv-scanner.toml` or `.github/osv-scanner.toml`, as configured by the repository's dependency workflow. Do not bypass required checks.

Public advisories are listed on the affected repository's Security tab. An empty advisory list does not establish that the software has no vulnerabilities.
