# Golang hooks for pre-commit

## Pre-requist:

### pre-commit
Install [pre-commit](https://pre-commit.com/#install)

### golangci-lint

Install [golangci-lint](https://golangci-lint.run/usage/install/)


## Usage

golangci-lint can be used as a hook for pre-commit, add on your `.pre-commit-config.yaml`

```
repos: 
  - repo: git@github.com:racken/golang-pre-commit-hooks.git
    rev: master
    hooks: 
      - id: golangci-lint
        args: ['--timeout 2m'] // optional
```
