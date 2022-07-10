## Release Please

Used for semi-automatically releasing new versions. Only relevant within CI/CD,
so no local setup required.

- <https://github.com/googleapis/release-please>
- <https://github.com/google-github-actions/release-please-action>

Configuration of Release Please fully takes in the GitHub Actions workflow
files, where Release Please is utilized via a dedicated GitHub Action.

## Cheat Sheet

### Add custom description before release

As of today (2022-07-10) it is not possible out of the box to add custom
description to the release notes and changelog before releasing. There's an
feature request open for this
[here](https://github.com/googleapis/release-please/issues/1274).

But there is a manual "hack" around this missing feature.

1. Checkout the pull request branch and update the changelog.
2. Edit the pull request description.
3. Merge the pull request.

Make sure to do this right before you are ready to release. Else the manually
injected content will be scrambled.
