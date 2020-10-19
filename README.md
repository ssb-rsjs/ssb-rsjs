# SSB Neon

> Migrating the SSB Node.js stack to Rust, gradually

SSB Neon modules are **npm packages** written in Rust instead of JavaScript. You can use the npm package `ssb-neon-something` as a direct replacement of `ssb-something`.

Currently, these are:

- [x] [`ssb-keys-neon`](https://github.com/staltz/ssb-keys-neon)
- [ ] `neon-muxrpc`
- [ ] `neon-multiserver`
- [ ] `ssb-neon-conn`
- [ ] `ssb-neon-tunnel`
- [ ] `ssb-neon-ref`
- [ ] `ssb-neon-blobs`
- [ ] `ssb-neon-serve-blobs`
- [ ] `ssb-neon-config`
- [ ] `ssb-neon-friends`
- [ ] `ssb-neon-replicate`
- [ ] `ssb-neon-ebt`
- [ ] `ssb-neon-validate`
- [ ] `neon-flumedb`
- [ ] `neon-flumelog-offset`
- [ ] `neon-flumeview-level`
- [ ] `neon-flumeview-query`
- [ ] `ssb-neon-backlinks`
- [ ] `ssb-neon-private`
- [ ] `ssb-neon-search`
- [ ] ([Help us tick these boxes!](./CONTRIBUTING.md))

## Contributing

If you want to create one of these modules, check the [Contributor guide](./CONTRIBUTING.md).

## Big picture plan

To read more on why and how we're building SSB Neon, check [The Plan](./PLAN.md).
