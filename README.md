# example-python

[![view-action-graph](https://img.shields.io/github/actions/workflow/status/actionforge/example-python/workflow.yml?label=View%20Action%20Graph)](https://app.actionforge.dev/github/actionforge/example-python/main/.github/workflows/graphs/build.act)

A simple Hello World app in Python, built using an [Actionforge](https://actionforge.dev) graph as the CI/CD pipeline.

## Run

```bash
python hello.py
```

## Graph

The build pipeline is defined as an Actionforge graph in [`.github/workflows/graphs/build.act`](.github/workflows/graphs/build.act):

```
checkout -> setup-python -> run (shell: python)
```

It runs on every push to `main`, on pull requests, and on manual dispatch.
