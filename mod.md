## Modified for [measure.sh](https://github.com/measure-sh/measure)

The `measure` branch contains all modifications. The `measure` branch should **NEVER** merge to `master`. Changes from upstream should **ALWAYS** merge to `master`.

## List of modifications

1. **GitHub Workflows** Sentry specific & other supportive workflows has been disabled.
    - Workflows that require Sentry specific secrets/variables has been disabled.
    - Tests that require Sentry specific secrets/variables has been disabled.

## Maintainance Guide

1. Don't push any change on `master`.
2. All measure.sh related changes should be pushed to `meaure` branch.
