---
layout: default
title: ursa
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/ursa
---

# ursa <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/ursa){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/220" class=".btn">#220</a>
            </td>
            <td>
                <b>
                    Bump bumpalo from 3.10.0 to 3.12.0 in /libursa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [bumpalo](https://github.com/fitzgen/bumpalo) from 3.10.0 to 3.12.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/fitzgen/bumpalo/blob/main/CHANGELOG.md">bumpalo's changelog</a>.</em></p>
<blockquote>
<h2>3.12.0</h2>
<p>Released 2023-01-17.</p>
<h3>Added</h3>
<ul>
<li>Added the <code>bumpalo::boxed::Box::bump</code> and <code>bumpalo::collections::String::bump</code>
getters to get the underlying <code>Bump</code> that a string or box was allocated into.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Some uses of <code>Box</code> that MIRI did not previously consider as UB are now
reported as UB, and <code>bumpalo</code>'s internals have been adjusted to avoid the new
UB.</li>
</ul>
<hr />
<h2>3.11.1</h2>
<p>Released 2022-10-18.</p>
<h3>Security</h3>
<ul>
<li>Fixed a bug where when <code>std::vec::IntoIter</code> was ported to
<code>bumpalo::collections::vec::IntoIter</code>, it didn't get its underlying <code>Bump</code>'s
lifetime threaded through. This meant that <code>rustc</code> was not checking the
borrows for <code>bumpalo::collections::IntoIter</code> and this could result in
use-after-free bugs.</li>
</ul>
<hr />
<h2>3.11.0</h2>
<p>Released 2022-08-17.</p>
<h3>Added</h3>
<ul>
<li>Added support for per-<code>Bump</code> allocation limits. These are enforced only in the
slow path when allocating new chunks in the <code>Bump</code>, not in the bump allocation
hot path, and therefore impose near zero overhead.</li>
<li>Added the <code>bumpalo::boxed::Box::into_inner</code> method.</li>
</ul>
<h3>Changed</h3>
<ul>
<li>Updated to Rust 2021 edition.</li>
<li>The minimum supported Rust version (MSRV) is now 1.56.0.</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/fitzgen/bumpalo/commit/50ba1bdd406665bd2e6ba430e167a38ed1b13964"><code>50ba1bd</code></a> Bump to 3.12.0</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/3dd36507db87e1b86617f1da88a9bc81374e7faf"><code>3dd3650</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/190">#190</a> from mattfbacon/main</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/37be9a98e4241a9cc6e534c47778cb2f4337b83f"><code>37be9a9</code></a> Merge branch 'fitzgen:main' into main</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/3664dbb7922fa1372adf53fb8767cd0fc2115267"><code>3664dbb</code></a> Add String::bump method</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/701514f553a6feab61b99e0382f314d532f57272"><code>701514f</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/189">#189</a> from mattfbacon/main</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/c6507f7a4c33811a275b357004c3904261c8908c"><code>c6507f7</code></a> Add Vec::bump method</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/b1e67b7aa188d4128343858bf86a29f1c99362c6"><code>b1e67b7</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/188">#188</a> from saethlin/field-retagging</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/d325e2c94576f6806508751f945ba5985661b721"><code>d325e2c</code></a> Use ManuallyDrop with bumpalo's Box instead of mem::forget</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/c699cd1303c441953344f354892b550df6c24aa1"><code>c699cd1</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/fitzgen/bumpalo/issues/183">#183</a> from stepancheg/allocated-bytes-no-headers</li>
<li><a href="https://github.com/fitzgen/bumpalo/commit/5805a293e8ba99f2adfd9c02ee6ad2532ad52fca"><code>5805a29</code></a> Clarify allocated_bytes does not include headers</li>
<li>Additional commits viewable in <a href="https://github.com/fitzgen/bumpalo/compare/3.10.0...3.12.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=bumpalo&package-manager=cargo&previous-version=3.10.0&new-version=3.12.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/ursa/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 22:14:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    Adding Roman Shanin as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shanin Roman <shanin1000@yandex.ru>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 15:14:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    Adding Aleksandr Petrosyan as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Brent Zundel <brent.zundel@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 16:13:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    fix(wasm): compilable and updated some of the bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Did some local testing and ed25519sha512 and bls seem to work.


```typescript
import { Ed25519Sha512 } from "ursa";
import assert from "assert";

// Test vectors from ursa/libursa/src/signatures/ed25519.rs

const message = new TextEncoder().encode(
  "This is a dummy message for use with tests"
);

const signature = Buffer.from(
  "451b5b8e8725321541954997781de51f4142e4a56bab68d24f6a6b92615de5eefb74134138315859a32c7cf5fe5a488bc545e2e08e5eedfd1fb10188d532d808",
  "hex"
);

const publicKey = Buffer.from(
  "27c96646f2d4632d4fc241f84cbc427fbc3ecaa95becba55088d6c7b81fc5bbf",
  "hex"
);

assert(Ed25519Sha512.verify(message, signature, publicKey));
```

bls has some issues, maybe intentional, with dropping values (see g1 and g2).
```typescript
import assert from "assert";
import { Bls, Generator, SignKey, VerKey } from "ursa";

const msg = new Uint8Array([1, 1, 1]);

const seed = new Uint8Array(32);
const b = new Generator().toBytes();

// Creating of the same two generators as `Bls.sign` drops one and `Bls.verify` as well.
const g1 = Generator.fromBytes(b);
const g2 = Generator.fromBytes(b);

const signKey = SignKey.fromSeed(seed);
const signKey2 = SignKey.fromSeed(seed);

const verKey = new VerKey(g1, signKey);
const signature = Bls.sign(msg, signKey2);

assert(Bls.verify(msg, signature, verKey, g2));
```

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-17 18:08:29 +0000 UTC
    </div>
</div>

