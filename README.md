# action-disable-apparmor #

[![GitHub Build Status](https://github.com/cisagov/action-disable-apparmor/workflows/build/badge.svg)](https://github.com/cisagov/action-disable-apparmor/actions)

A GitHub Action to disable AppArmor on the GitHub runner.

## Usage ##

### Inputs ###

None.
<!--
| Name | Description | Interpreted Type | Default | Required |
|------|-------------|------------------|---------|:--------:|
| input_name | The input's description. | `string` | n/a | yes |
-->

### Outputs ###

None.
<!--
| Name | Description | Output Type |
|------|-------------|-------------|
| output_name | The output's description. | `output_type` |
-->

### Sample GitHub Actions workflow ###

This GitHub Action only makes changes to the runner and therefore
requires no permissions.

```yml
---
name: The workflow

on:
  pull_request:
  push:

jobs:
  my_job:
    # This job does not need any permissions
    permissions: {}
    runs-on: ubuntu-latest
    steps:
      - name: Disable AppArmor on the GitHub runner
        uses: cisagov/action-disable-apparmor@develop
```

## Contributing ##

We welcome contributions!  Please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for
details.

## License ##

This project is in the worldwide [public domain](LICENSE).

This project is in the public domain within the United States, and
copyright and related rights in the work worldwide are waived through
the [CC0 1.0 Universal public domain
dedication](https://creativecommons.org/publicdomain/zero/1.0/).

All contributions to this project will be released under the CC0
dedication. By submitting a pull request, you are agreeing to comply
with this waiver of copyright interest.
