# oss

The ten public repositories of synapt's open-source stack, kept together as one workspace:

| Repository | What it is |
|---|---|
| [grip](https://github.com/synapt-dev/grip) | Multi-repository workspace and review tooling (`gr2`) |
| [recall](https://github.com/synapt-dev/recall) | Persistent memory for AI coding assistants |
| [runner](https://github.com/synapt-dev/runner) | Research-runner kernel: run records, hashing, gates, artifacts |
| [eval](https://github.com/synapt-dev/eval) | Eval framework: runners, report cards, PR gates |
| [extract](https://github.com/synapt-dev/extract) | Structured extraction schema, types and validation for AI agents |
| [codi](https://github.com/synapt-dev/codi) | AI coding assistant supporting Claude, OpenAI and local models |
| [codi-rs](https://github.com/synapt-dev/codi-rs) | Rust implementation of Codi |
| [codememo-benchmark](https://github.com/synapt-dev/codememo-benchmark) | Reproducible CodeMemo benchmark, with pinned versions |
| [vorn-mat](https://github.com/synapt-dev/vorn-mat) | The Vorn paper with its reproducible code, data and figures |
| [homebrew-tap](https://github.com/synapt-dev/homebrew-tap) | Homebrew formulae for synapt tools |

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
gr2 store materialize   # clones the ten at their pinned commits
gr2 store check
```
