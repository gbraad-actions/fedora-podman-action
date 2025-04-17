Fedora container Action (podman)
================================


Run commands in a Fedora container environment using Podman


## Usage

```yaml
name: Test

on:
  workflow_dispatch:

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - name: Say moo
        uses: gbraad-actions/fedora-podman-action@main
        with:
          dnf-packages: cowsay
          run: |
            cowsay Hello
```
