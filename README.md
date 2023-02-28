## Reusable workflows

### CODEOWNERS Extension

To call [this workflow](.github/workflows/codeowners-check.yml):

```yaml
name: Codespaces Check
on:
  pull_request:
    branches: [ "main" ]
jobs:
  caller:
    uses: boxboat/reusable-workflows/.github/workflows/codeowners-check.yml@main
    secrets: inherit
```
