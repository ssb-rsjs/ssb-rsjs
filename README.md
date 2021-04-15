# SSB Neon

> Migrating the SSB Node.js stack to Rust, gradually

SSB RSJS modules are **npm packages** written in Rust instead of JavaScript. You can use the npm package `ssb-something-rsjs` as a direct replacement to `ssb-something`.

Currently, these are:

- [x] [`ssb-keys-neon`](https://github.com/staltz/ssb-keys-neon)
- [x] [`ssb-keys-mnemonic-neon`](https://github.com/staltz/ssb-keys-mnemonic-neon)
- [ ] `pull-box-stream-rsjs`
- [ ] `secret-handshake-rsjs`
- [ ] `muxrpc-rsjs`
- [ ] `multiserver-rsjs`
- [ ] `ssb-conn-rsjs`
- [ ] `ssb-tunnel-rsjs`
- [ ] `ssb-ref-rsjs`
- [ ] `ssb-blobs-rsjs`
- [ ] `ssb-serve-blobs-rsjs`
- [ ] `ssb-config-rsjs`
- [ ] `ssb-friends-rsjs`
- [ ] `ssb-replicate-rsjs`
- [ ] `ssb-ebt-rsjs`
- [ ] `ssb-validate-rsjs`
- [ ] `async-append-only-log-rsjs`
- [ ] `jitdb-rsjs`
- [ ] `ssb-db2-rsjs`
- [ ] `ssb-threads-rsjs`
- [ ] `ssb-private-rsjs`
- [ ] ([Help us tick these boxes!](./CONTRIBUTING.md))

## Contributing

If you want to create one of these modules, check the [Contributor guide](./CONTRIBUTING.md).

## Big picture plan

To read more on why and how we're building SSB RSJS, check [The Plan](./PLAN.md).
