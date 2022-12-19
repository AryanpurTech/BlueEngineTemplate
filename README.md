# Template for [Blue Engine](https://github.com/AryanpurTech/BlueEngine)

This is a template to get you up and running faster. It has fast build time by default, with option to change it to normal build upon release, and some other goodies.

## Getting started

Just clone the repository:

```bash
git clone https://github.com/AryanpurTech/BlueEngineTemplate
```

For the fast build times:

### Linux

You are good to go, just continue using normally.

### Windows

Rename the `.cargo-win` to `.cargo`, and set the current workspace as nightly:

```bash
rustup override set nightly
```

And you are now good to go.

## Release builds

for release builds, all you need to do is in the `Cargo.toml`, change the `blue_engine`'s `path="./blue_engine"` option with `version="0.4"`. That's it. It'll build most optimized version for release. When going back to debugging, change it back to original `path="./blue_engine"`.

## What's the difference?

Things that have been added are:

* in the `blue_engine`, the crate type has been set to `dylib`.
* release profile have been added some optimizations to.
* for windows, some extra settings have been applied to to enable `dylib`.

If you'd like to apply it yourself, check out the [wiki](https://aryanpurtech.github.io/BlueEngineDocs/first_chapter/setup.html#turbo-build-times).
