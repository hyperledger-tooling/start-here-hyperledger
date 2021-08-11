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
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Bump path-parse from 1.0.6 to 1.0.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [path-parse](https://github.com/jbgutierrez/path-parse) from 1.0.6 to 1.0.7.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/jbgutierrez/path-parse/commits/v1.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=path-parse&package-manager=npm_and_yarn&previous-version=1.0.6&new-version=1.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 22:54:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Refactored crypto & client; publishment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Crypto now exposes the same API as the origin `iroha_crypto` crate.
- Refactored client exposes more low-level API to provide a better control of transaction building process.

## Unresolved problems

### `@iroha/crypto` is only ESM-compatible

Usage of `@iroha/crypto` is still not very clear and requires a native ES modules environment. In web it works fine with `vite`, and also in node with `esbuild-register`. Other cases are not very well researched.

### `iroha_crypto_core` crate

> Located at `packages/iroha-crypto/rust/iroha_crypto_core`

It is a copy of `iroha_crypto` crate from [hyperledger/iroha (iroha2-dev)](https://github.com/hyperledger/iroha/tree/iroha2-dev) repo, refactored to be no-std compatible. The better way to make it I see here is to refactor the main crate to be no-std compatible and use it directly in `iroha_crypto_wasm` crate in this repo.

### Don't forget to `free()` crypto structures!

They will never be garbage collected manually, so if you don't want memory leaks, you have to `free()` every created structures manually when they have to be dropped.

### Inefficiency of exposed API by `wasm_bindgen`

There is a lot of data cloning that looks like unnecessary, but I can't determine and don't know how to design it in better way. Maybe we will see it after some real-world usage.

Also, `wasm_bindgen` has some undocumented behavior (or I haven't found any documentation) - Rust's ownership rules works on incoming exposed structures! For example:

```rust
#[wasm_bindgen]
pub struct PublicKey {
    payload: Vec<u8>
}

#[wasm_bindgen]
impl PublicKey {
    #[wasm_bindgen(constructor)]
    pub fn new() -> PublicKey {
        PublicKey { payload: vec![] }
    }
}

#[wasm_bindgen]
pub fn get_pub_key_payload(val: PublicKey) -> Vec<u8> {
    val.payload
}
```

This will be compilted to JS-wrappers like this:

```ts
declare export class PublicKey {
    free(): void;
    constructor();
}

declare export function get_pub_key_payload(val: PublicKey): UInt8Array;
```

And when you use it like this:

```ts
// new struct, memory allocated
const pk = new PublicKey();


const bytes = get_pub_key_payload(pk);
//                                ^^ here `pk` is moved, and we can't use it anymore in JS

// trying to use `pk` again...
get_pub_key_payload(pk); // error! null pointer passed to rust
```

So, OK, ownership rules affect generated bindings with `wasm_bindgen`, **but it is completely unclear from the JS side!** There is no any borrow-checker in JS that will fail compilation in case when ownership rules have been violated. So I removed all cases when incoming values are being *moved* and I always *borrow* them and copy when it is necessary.

How to solve it? Idk, maybe we have to completely redesign the WASM crate to exclude any possibility to use it improperly. We need more usage examples.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-07 08:46:12 +0000 UTC
    </div>
</div>

