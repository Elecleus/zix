# zix

## Description
A reimagining of Nix that aims to address several of Nix's drawbacks, such as its non-FHS store layout, steep learning curve, and other usability issues.

## Inspiration
- [**Nix**](https://nixos.org): for its strong declarative model.
- [**Guix**](https://guix.gnu.org): for design differences that provide useful alternatives.
- [**Apache BuildStream**](https://www.buildstream.build): for its container and layer-based build process.

## Current ideas / design goals
- Content organized as `layers` in the store.
- Build processes separated into `process` units, forming pipeline-like stages with well-defined inputs and outputs.
- A uniform, extensible configuration data structure that provides a consistent modification API.
- Use OverlayFS for building and composing layers.
- Provide processes to copy or link artifacts from the store.
- May leverage [bootc](https://github.com/bootc-dev/bootc) where appropriate.

## Links that may be useful
- [nix2container](https://github.com/nlewo/nix2container)
- [ciel](https://github.com/AOSC-Dev/ciel-rs)
- [Universal Blue Project](https://github.com/ublue-os) — examples of distributions that already use `bootc`