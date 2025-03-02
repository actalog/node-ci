# @actalog/node-ci

[![CI](https://github.com/actalog/node-ci/actions/workflows/ci.yml/badge.svg)](https://github.com/actalog/node-ci/actions/workflows/ci.yml)
[![CD](https://github.com/actalog/node-ci/actions/workflows/cd.yml/badge.svg)](https://github.com/actalog/node-ci/actions/workflows/cd.yml)

Continuous Integration for Node.js projects

## Getting started

```yml
name: CI

on:
  - pull_request
  - push

permissions:
  pull-requests: write

jobs:
  node-ci:
    name: Node CI
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actalog/node-ci@v3
```
