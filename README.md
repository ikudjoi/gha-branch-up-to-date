# gha-branch-up-to-date
Composite GitHub action that checks whether the pull request branch is up-to-date with the base branch.

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
      base-ref: your-pr-base-branch-ref
      fail: false
```