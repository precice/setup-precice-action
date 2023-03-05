# setup-precice-action

This action installs preCICE in the given prefix and adds it to the path.

## Inputs

### `precice-version`

The version of preCICE to use. Can be a branch or tag or SHA. Defaults to `develop`

### `install-prefix`

The installation prefix for preCICE. Default is `/usr/local`

### `build-tests`

Whether to build tests. Should be `OFF` off for all non-develop builds. Defaults to `OFF`

## Example usage

```yml
- name: build preCICE
  uses: precice/setup-precice-action@main
  with:
    precice-version: develop
    install-prefix: /usr/local
```