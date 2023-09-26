# 🛠️ Foundry Pre-Commit Hook 🪝

Run [Foundry](https://github.com/foundry-rs/foundry) `forge fmt` and/or `forge snapshot` before
commit.

## Usage

1. Install [Foundry](https://book.getfoundry.sh/getting-started/installation).
2. Install [`pre-commit`](https://pre-commit.com/#install).
3. Add the following to `.pre-commit-config.yaml` in your repo.

```yaml
repos:
    - repo: https://github.com/0xvangrim/foundry-pre-commit
      rev: v1.0.0
      hooks:
          - id: format
          - id: snapshot
```

4. Run `pre-commit install` to set up the hooks.
5. 🎉 From now on, before each commit, `forge fmt` will be ran automatically.

## NOTE
You can find all the hooks here that you can use here: https://pre-commit.com/#cli