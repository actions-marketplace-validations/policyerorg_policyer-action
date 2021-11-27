# policyer-action

Policyer Github action.

For more details visit [policyer](https://github.com/niradler/policyer)

## usage

```yaml
name: Policyer

on: [pull_request]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Policyer GitHub Action
        uses: policyerorg/policyer-action@v0.0.3-alpha
        with:
          verbose: false
          provider: policyer-github
          internal: false
          checks_path: ./checks        
```