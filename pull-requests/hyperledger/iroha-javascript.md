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
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Fix packages: paths (ts & jest), versions, changelogs etc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove paths from tsconfig and jest config - now direct imports from `"main": "src/lib.ts"` in `package.json`;
- Setup publish configs for each non-private package in `publishConfig` field of each `package.json`;
- Set `"private": true` for each of internal packages - test sub-packages of `crypto`, `@iroha2/test-peer`, `@iroha2/monorepo`;
- Make names of packages dirs consistent - remove `iroha-` prefix (so there a lot of just renamed files);
- Update dependencies;
- Setup `changesets` for version control.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 08:26:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    Different entrypoints in `@iroha2/crypto`  & dependency inversion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## The problem

> At this point in time deploying Rust and WebAssembly to the web or other locations unfortunately isn't a trivial task to do.
> *[`wasm-pack` docs about deployment](https://rustwasm.github.io/docs/wasm-bindgen/reference/deployment.html)*

Before this I was sure that `web` target works fine both in web and nodejs environment, and it was! But unfortunately not in all cases and with some reservations and pitfalls. It is ok, so why not just expose different entrypoints in the same library? Because such approach produces huge problems for the libraries that would depend on this one and be target-agnostic, e.g. `@iroha2/client` pkg.

## The solution

In this PR library contains main "types" entrypoint in `/types` and target-specific ones in sub-directories. It has the main type - `IrohaCryptoInterface`, and each target-specific implementation exports the same `crypto` object that is compatible with this type (it is included into type-check of the monorepo as test). And with this type it is possible to write libraries that depends on it and injects a particular implementation in runtime.

## What not to check

`wasm-pack` outputs at `packages/iroha-crypto/(web|node|bundler)` dirs. Btw there are `index.js` and `index.d.ts` files generated separately from it but also automatically.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-26 16:55:54 +0000 UTC
    </div>
</div>

