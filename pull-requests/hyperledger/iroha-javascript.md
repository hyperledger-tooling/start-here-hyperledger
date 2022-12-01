---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    [feature]: functional approach to compile data-model artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Old approach

Iroha JavaScript uses the original Iroha repository for a set of reasons:

- Run `kagami` in order to generate data-model schema
- Use `iroha_data_model` crate in order to generate encoded samples for data-model tests
- Run `iroha` binary in end-2-end tests

**Previously**, `iroha_data_model` was referenced in `packages/data-model-rust-samples/Cargo.toml` as:

```toml
iroha_data_model = { git = "<git repo>", rev = "<rev>" }
```

`kagami` and `iroha` binaries were built via `cargo build`:

```bash
cargo build --git "<git repo>" --rev "<rev>" --package kagami
```

This pipeline was encapsulated into `@iroha2/dev-iroha-bins` package and was semi-automatic - compiled artifacts were produced and committed manually as described at ["Manually update reference iroha version"](https://github.com/hyperledger/iroha-javascript/tree/iroha2#manually-update-reference-iroha-version) guide.

## New approach

### Automatic updates of the reference iroha in a single place

`@iroha2/iroha-source` dev packages comes in instead of `@iroha2/dev-iroha-bins`. In order to change reference Iroha version, it is only needed to update `packages/iroha-source/config.json`, and everything else will be re-compiled on the fly.

The configuration schema is pretty straightforward:

```json
{
  "origin": "https://github.com/hyperledger/iroha.git",
  "rev": "52dc18cd81bdc1d1906ffeecb666dd9b2eb27955"
}
```

These parameters are used to `git clone` the repo. Thus, `origin` field might be even a file-system path, and `rev` - a branch/tag name.

Then, each time when some actor needs to use `iroha` or `kagami` binary, the following steps are performed:

```ts
import { resolveBinary } from '@iroha2/iroha-source'

const irohaPath = (await resolveBinary('iroha')).path
// 1. If the repo is not cloned, clone it. If the cloned repo is not the same as specified
//    in `config.json`, update it.
// 2. If there is no `target/release/iroha`, run `cargo build --release --package iroha`
// 3. Return path to the `target/release/iroha` binary
```

Also, `data-model-rust-samples` crate now references `iroha_data_model` via `path` option in `Cargo.toml`, which:

- Removes the need to manually duplicate Iroha git reference as it was before;
- Leverages compilation cache in the cloned repo.

### Exclude data-model artifacts from Git tracking

Those artifacts aren't tracked by Git anymore:

- `packages/data-model-schema/src/__schema__.json`
- `packages/data-model-rust-samples/samples.json`
- `packages/data-model/src/__generated__.ts`

Their generation now works fast, and it is run at following steps:

- Monorepo `postinstall` script
- Before tests and build

### Refactored monorepo tasks

I made some changes in the root Jakefile and `package.json`. Notable ones:

- At the `postinstall` step, data-model artifacts are compiled
- `pnpm publish-all` now runs all necessary steps, including tests and build.

-----

In conclusion, the overall approach is easier to use, maintain and is more robust, because now it is harder to "forget" update data-model schema - it updates automatically before each step that needs it, and it runs fast in dev environment.

However, CI/CD might run longer now, because it will compile 3 Rust crates, but this process is optimized thanks to incremental compilation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 05:17:08 +0000 UTC
    </div>
</div>

