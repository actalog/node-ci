# Node CI

Continuous Integration for Node.js projects

## Getting started

```yml
name: CI

on:
  - push

jobs:
  node-ci:
    name: Node CI
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: gabrielrufino/node-ci@v1
```
