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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-26 16:55:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    fix: bundle cjs script for crypto lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now it should work in node without on-demand transformations like `esbuild-register` or `sucrase/register`. But the way it is done now is not the best... FIXME

Version bumps:

- `@iroha2/client` - 0.2.0 -> 0.2.1
- `@iroha2/crypto` - 0.1.0 -> 0.2.0

#### Breaking changes

Only one - initialization way:

```ts
// was
import init from '@iroha2/crypto'

// now
import { init } from '@iroha2/crypto'
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 11:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Bump `@iroha2/client` version to 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Forgot to do it in previous PR (
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 13:27:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    Update data model with new SCALE codec compiler, actualize client code, implement `Fixed`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 12:44:27 +0000 UTC
    </div>
</div>

