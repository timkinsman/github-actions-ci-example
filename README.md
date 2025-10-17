# github-actions-ci-example
GitHub Actions setup for CI

### tests.yml

Runs `build`, `lint` and `test` scripts on `develop` branch pull_request events and `main` branch push&pull_request events.

### bump-version.yml

Bumps the package.json version on a successful `tests.yml` run on a `main` branch push event.

### release.yml

Creates a github tag and release on a successful `bump-version.yml` run on a `main` branch.
