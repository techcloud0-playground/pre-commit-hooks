# pre-commit-hooks

## Getting started

### Install pre-commit

See [https://pre-commit.com/#install](https://pre-commit.com/#install).

### Configure pre-commit

Create a similar file shown in below content named `.pre-commit-config.yaml` at the root of your repository.

```yaml
repos:
  - repo: https://github.com/techcloud0-playground/pre-commit-hooks
    rev: <VERSION> # https://github.com/techcloud0-playground/pre-commit-hooks/releases
    hooks:
      - id: keep-sorted
      # See `.pre-commit-hooks.yaml` for available hooks.
```

### Install hooks

```shell
pre-commit install
```

## Development

### Uninstall hooks

```shell
pre-commit uninstall -t pre-commit -t pre-merge-commit -t pre-push -t prepare-commit-msg -t commit-msg -t post-commit -t post-checkout -t post-merge -t post-rewrite
```

### Clear cache

```shell
rm --force --recursive ~/.cache/pre-commit
```
