# Google Summer of Code 2019: Kapitan new features

This page describes the work I have done over the course of three months (May to August) as a participant of Google Summer of Code (GSoC) 2019. I was a student under [deepmind/kapitan](https://github.com/deepmind/kapitan), mentored kindly by Pawel, Ricardo and Adrian. The original proposal can be found in this repository for reference as well.

## Implemented features

### Feature 1: External dependency management

This feature allows Kapitan to pull external sources/components from a remote location during compile, as described in [this issue](https://github.com/deepmind/kapitan/issues/91). The documentation can be found [here](https://kapitan.dev/external_dependencies/).

This feature has been merged. The code can be found in this [PR](https://github.com/deepmind/kapitan/pull/304) on Github.

### Feature 2: Helm input type

This creates the Python binding to `helm template` command written in Golang such that users can render helm templates as a new input type to kapitan. The original issue is found [here](https://github.com/deepmind/kapitan/issues/143). The documentation is available [here](https://kapitan.dev/compile/#helm).

This feature has been merged. The code can be found in this [PR](https://github.com/deepmind/kapitan/pull/307) on Github.

### Feature 3: Manifest validation

This feature allows users to validate compiled output against json schemas such that they can confirm whether the compiled output is valid manifest for kubernetes. This original issue is found [here](https://github.com/deepmind/kapitan/issues/194). The documentation is available [here](https://kapitan.dev/validate/).

This feature has been merged. The code can be found in this [PR](https://github.com/deepmind/kapitan/pull/317) on Github.

### Feature 4: standalone binary

Kapitan has been available via pip or docker. A standalone binary for Linux systems has been created using Pyinstaller which ships the Python interpreter as well so that it can even run on systems without Python runtime.

## Extra stuff

- Secret sub-variables feature that allows multiple secrets to be stored in a single yaml file (Merged):  <https://github.com/deepmind/kapitan/pull/282>
- Creating a more structured documentation using mkdocs (Merged): <https://github.com/deepmind/kapitan/pull/331>