# Setup Bloc Tools

[![ci](https://github.com/felangel/setup-bloc-tools/actions/workflows/main.yaml/badge.svg)](https://github.com/felangel/setup-bloc-tools/actions/workflows/main.yaml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)

Installs and sets up [`bloc command-line tools`](https://pub.dev/packages/bloc_tools) for use in GitHub Actions.

This action:

1. Downloads the Dart SDK
1. Adds the `dart` tool to the system path
1. Activates the `bloc_tools` CLI

## Usage

```yml
name: Bloc
on: pull_request

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: felangel/setup-bloc-tools@v0
      - run: bloc --version
```
