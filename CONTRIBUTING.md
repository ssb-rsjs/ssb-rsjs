# Contributor guide

## This org does not hold repositories

You may have noticed that no Neon module is published under `https://github.com/ssb-neon`. This is intentional. We do not want to centralize the SSB Neon modules in this org because we do not yet care about code quality or consistency or consensus. You are free to host your SSB Neon module under your own name, follow whatever maintenance style you prefer. **We don't want to get in your way** of being productive. While we're still in [Horizon 1](./PLAN.md), we only care about one thing:

## Curation of backwards compatibility

In order to get your new SSB Neon module listed in the `ssb-neon` README.md, we only demand a couple requirements:

- `ssb-neon-something` was built from the `neon new ssb-neon-something` CLI
- `ssb-neon-something` JavaScript implementation is only very few lines of code
- `ssb-neon-something@X.Y.Z-num` is backwards compatible with `ssb-something@X.Y.Z`
- `ssb-neon-something@X.Y.Z-num` passes all tests from `ssb-something@X.Y.Z`'s test suite
- `ssb-neon-something` can be used as a drop-in replacement to `ssb-something` in at least one of these apps: Patchwork, Patchbay, Oasis, Manyverse
- Replacing `ssb-something` with `ssb-neon-something` requires changing only very few lines of code

If your Neon module passes these requirements, that's all we need to list it in the README!

## Ideally...

These are not rules for contribution, they are just suggestions how to write your SSB Neon module:

- Try to publish core SSB logic as Rust crates
- Import those crates in your SSB Neon module
- The Rust code in `ssb-neon-something` should ideally only handle JS inputs, handle error cases in JS, delegate logic to SSB Rust crates, and convert Rust output to JS output
- Your module is published on npm with a `prebuilds` folder (see [neon-tag-prebuild](https://github.com/staltz/neon-tag-prebuild) and [neon-load-or-build](https://github.com/staltz/neon-load-or-build))
- Your module can be consumed either from npm or from git (e.g. see these [two usage options](https://github.com/staltz/ssb-neon-keys#usage) in `ssb-neon-keys`)
