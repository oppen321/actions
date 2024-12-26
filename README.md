# Install LLVM/CLANG on Github Action (ubuntu)

## Usage

```yaml
name: Test
on: push

jobs:
  build:
    name: Test
    runs-on: ubuntu-24.04
    steps:
      - name: Checkout
        uses: actions/checkout@main

      - name: Install LLVM
        uses: oppen321/actions@install-llvm

      - name: Test
        run: |
          clang --version
```
