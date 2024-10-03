## Modified for [measure.sh](https://github.com/measure-sh/measure)

The `measure` branch contains all modifications. The `measure` branch should **NEVER** merge to `master`. Changes from upstream should **ALWAYS** merge to `master`.

## List of modifications

1. **GitHub Workflows** Sentry specific & other supportive workflows has been disabled.
    - Workflows that require Sentry specific secrets/variables has been disabled.
    - Tests that require Sentry specific secrets/variables has been disabled.

## Maintainance Guide

1. Don't push any change on `master`.
2. All measure.sh related changes should be pushed to `measure` branch.
3. To send changes to upstream, follow these steps.
    - Sync master branch with upstream's master
    - Create a new branch
    - Make changes and run tests on local machine
    - Push changes to newly created branch
    - Open a Pull Request to upstream's master from your branch
    - Once upstream has merged, sync master with upstream's master
    - Delete created branch
4. To release a new version, follow these steps.
    - Follow semver starting from `1.0.0`
    - Create a new `release/*` branch. For example: `release/1.0.0`
    - Merge `measure` to newly created branch
    - Push release branch and wait until workflows succeed
    - Test the newly released docker image/artifacts/binaries
    - Backmerge the release branch to `measure` branch
    - Delete the release branch
