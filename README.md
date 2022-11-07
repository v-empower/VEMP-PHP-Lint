# GitHub Action for PHPLint

GitHub Action implementation of the PHPLint Package

## Usage

Use with [GitHub Actions](https://github.com/features/actions)

_.github/workflows/phplint.yml_

```
name: PHP Linting
on: pull_request
jobs:
  phplint:
    runs-on: ubuntu-latest
    steps:
        - uses: actions/checkout@v1
        - uses: v-empower/VEMP-PHP-Lint@master
```

If provided, a `.phplint.yml` file in the root will be used for configuration during run of the Action.