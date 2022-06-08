# github-workflows
Workflow and actions used for Monarch and Front Desk Station CI

## Usage examples
### Workflows
```yaml
name: Bump version
  uses: runslikebutter/github-workflows/.github/workflows/bump-version.yml@v7
  with:
    branch: develop
  secrets:
    GITHUB_BUILD_TOKEN: ${{ secrets.SOME_BUILD_TOKEN }}
```

### Actions
```yaml
name: Prep and install dependencies
  uses: runslikebutter/github-workflows/actions/install-dependencies@v7
  with:
    ssh_key: ${{ secrets.SOME_SSH_KEY }}
```