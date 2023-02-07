# gha-branch-up-to-date
Composite GitHub action that checks whether the pull request branch is up-to-date with the base branch.
Checks whether the diff between prospective merge commit and the head branch is empty.

Requires the contents read permission to your workflow:

```yaml
permissions:
  contents: read
```

# usage

```yaml
  - uses: ikudjoi/gha-branch-up-to-date@main
    with:
      head-ref: your-pr-head-branch-ref
      merge-commit-sha: SHA of the GitHub test merge commit
      fail: false
```