# Security Policy

## Supported versions

Unless a repository states otherwise, security fixes are provided for the **latest release**
and for `main`. Older releases may receive fixes at our discretion.

## Reporting a vulnerability

**Please do not report security vulnerabilities through public GitHub issues, discussions or pull requests.**

Use GitHub's private vulnerability reporting instead: open the repository's **Security** tab and click
**"Report a vulnerability"**. If that is unavailable for the repository in question, report it through
the private vulnerability form of the [LLCForge/LLCForge](https://github.com/LLCForge/LLCForge/security) repository.

Please include:

- the affected project and version/commit,
- a description of the issue and its impact,
- steps or a proof of concept to reproduce it,
- any suggested fix, if you have one.

## What to expect

| Step | Target time |
|---|---|
| Acknowledgement of your report | within 72 hours |
| Initial assessment and severity rating | within 7 days |
| Fix or mitigation for confirmed issues | depends on severity; critical issues are prioritised over all other work |
| Public advisory and credit | after a fix is released, coordinated with you |

We follow coordinated disclosure: we ask that you give us a reasonable time to fix the issue before
publishing details. We will credit you in the advisory and release notes unless you prefer to stay anonymous.

## Scope

Vulnerabilities in the source code, build pipeline, release artifacts and default configurations of
LLCForge projects are in scope. Issues in third-party dependencies should be reported upstream; let us
know as well so we can ship an updated dependency quickly.
