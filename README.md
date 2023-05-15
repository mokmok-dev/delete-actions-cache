# delete-actions-cache

GitHub Actions for delete Actions cache

## Usage

```yaml
name: delete actions cache
on:
  push:
    branches:
      - main
jobs:
  clean:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: mokmok-dev/delete-actions-cache@main
        with:
          github-token: ${{ secrets.GITHUB_TOKEN }}
```


See [action.yml](action.yml) for more details on how to configure it.
