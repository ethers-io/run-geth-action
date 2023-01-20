Run Geth
========

This action will install Geth and run a clique instance
in dev mode.

Configuration
-------------

**workflow.yml**

name: Run Geth

on:
  push:
    bracnhes:
      - master

jobs:

  run-geth:
    name: Run Geth

    runs-on: ubuntu-latest

    steps:
      - name: Use Node.js 16.x
        uses: actions/setup-node@v1
        with:
          node-version: 16.x

      - name: Checkout repository
        uses: actions/checkout@v2

      - name: Run Geth
        uses: ethers-io/run-geth-action

        
License
-------

MIT License.
