# oss

The four public repositories of synapt's open-source stack, kept together as one workspace:

| Repository | What it is |
|---|---|
| [grip](https://github.com/synapt-dev/grip) | Multi-repository workspace and review tooling (`gr2`) |
| [recall](https://github.com/synapt-dev/recall) | Persistent memory for AI coding assistants |
| [runner](https://github.com/synapt-dev/runner) | Research-runner kernel: run records, hashing, gates, artifacts |
| [eval](https://github.com/synapt-dev/eval) | Eval framework: runners, report cards, PR gates |

This repository holds no code of its own. `workspace.toml` declares the four, and `grip.toml` with the four submodules records the commit each one is pinned to.

## With git

```bash
git clone --recurse-submodules https://github.com/synapt-dev/oss.git
```

Each repository is checked out at its pinned commit.

## With gr2

```bash
pip install --pre gitgrip
git clone https://github.com/synapt-dev/oss.git
cd oss
gr2 store materialize   # clones the four at their pinned commits
gr2 store check
```
