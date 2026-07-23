# Contributing

Thanks for your interest in improving The WP Squad's projects! Contributions of all kinds are welcome — bug reports, reproductions, documentation fixes, and code.

This guide applies org-wide. An individual repository may add its own `CONTRIBUTING.md` with more specific instructions, which takes precedence.

## Where our code lives

Most of our development happens in private repositories, but a couple are public and open to contributions:

- **[squad-modules-lite](https://github.com/thewpsquad/squad-modules-lite)** — source mirror and issue tracker for Squad Modules Lite.
- **[freemius-wp-rest](https://github.com/thewpsquad/freemius-wp-rest)** — reusable WordPress REST API proxy routes for the Freemius SDK.

## Reporting bugs

Open an issue on the relevant repository and include:

- the product and version,
- your environment — WordPress, PHP, and Divi/Extra/Divi Builder versions,
- clear steps to reproduce,
- what you expected vs. what happened, and
- screenshots or a short screen recording where it helps.

Found a security vulnerability? **Do not open a public issue** — follow [SECURITY.md](SECURITY.md) instead.

## Suggesting features

Open an issue describing the problem you're trying to solve and the outcome you'd like. Real use cases help us prioritize far more than a bare feature name.

## Submitting code

1. **Fork** the repository and create a branch from the default branch.
2. Use a descriptive branch name, e.g. `fix/module-spacing` or `feat/new-option`.
3. **Match the code style.** Our WordPress code follows the [WordPress Coding Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/) (WPCS). If a repo ships a `composer.json` with lint tooling, run it before pushing:
   ```bash
   composer install
   composer lint      # PHPCS
   composer analyse   # PHPStan, where configured
   ```
4. Keep pull requests **focused** — one logical change per PR is easiest to review.
5. Write clear commit messages. We use [Conventional Commits](https://www.conventionalcommits.org/) prefixes (`feat:`, `fix:`, `docs:`, `chore:` …).
6. Open the pull request against the default branch and describe **what** changed and **why**.

## Code of conduct

By participating, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

Thank you for helping make our tools better for the whole Divi community. 💜
