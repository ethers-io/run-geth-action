Install and Run Geth
====================

This action will install Geth and run a clique instance
in dev mode.

Configuration
-------------

**workflow.yml**

```javascript
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
      - name: Install and run Geth
        uses: ethers-io/run-geth-action
```
        
License
-------

MIT License.
