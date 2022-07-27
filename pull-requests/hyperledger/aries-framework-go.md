---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3303" class=".btn">#3303</a>
            </td>
            <td>
                <b>
                    feat: mediator supports didcomm v1/v2 per-connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 19:02:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3296" class=".btn">#3296</a>
            </td>
            <td>
                <b>
                    test: interop jwt vc ecdsa
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
        Created At 2022-07-25 12:10:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3295" class=".btn">#3295</a>
            </td>
            <td>
                <b>
                    feat: Connection protocol (RFC-0160) DIDCommV1 implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
[Connection](https://github.com/hyperledger/aries-rfcs/tree/main/features/0160-connection-protocol#0160-connection-protocol) protocol (RFC-0160) DIDCommV1 implementation

**Summary:**

- On this PR only part related to protocol package is implemented (client part is not implemented yet)
- Also package called as `didconnection` because `connection` name is already used


closes https://github.com/hyperledger/aries-framework-go/issues/3299
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 11:38:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3294" class=".btn">#3294</a>
            </td>
            <td>
                <b>
                    feat: implement did-core JSON-LD `@context` representation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Abernethy <brownoxford@gmail.com>

**Title:**
Implement did-core JSON-LD `@context` representation

**Description:**
Current implementation assumes `@context` can only be `[]string`, but did-core v1 defines `@context` for DID documents in JSON-LD representation to be either a string or a list containing maps and/or strings.

**Summary:**
* Created `type Context {}interface` to represent did document contexts with appropriate comment for IDE integration.
* Modified `did.parseContext` to add parsing of `string` and `[]interface{}` context representations.
* Added `LookupContextString` helper to search for context string through entire context (used by `requiresLegacyHandling`)
* Added `LookupSchemaFromContext` helper to peek first string in context. Replaces direct references to `context[0]`
* Modified existing tests to account for new context format
* Added tests for new helper functions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 20:35:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3293" class=".btn">#3293</a>
            </td>
            <td>
                <b>
                    fix: bdd test ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 19:21:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3291" class=".btn">#3291</a>
            </td>
            <td>
                <b>
                    feat: allow custom GNAP header signer in vcwallet command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 19:10:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3286" class=".btn">#3286</a>
            </td>
            <td>
                <b>
                    test: interop jwt VCs tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds tests to ensure AFGO does support JWT VC parsing/verificaition by adding interop tests using VCs from external sources.
Also part of this change: expose JWT needed jose verifiers and signers for external use.

closes #3279

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 15:16:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3285" class=".btn">#3285</a>
            </td>
            <td>
                <b>
                    chore(deps): bump terser from 4.8.0 to 4.8.1 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 4.8.0 to 4.8.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v4.8.1 (backport)</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=4.8.0&new-version=4.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 20:50:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3284" class=".btn">#3284</a>
            </td>
            <td>
                <b>
                    feat: Size computation for allocation may overflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Performing calculations involving the size of potentially large strings or slices can result in an overflow (for signed integer types) or a wraparound (for unsigned types). An overflow causes the result of the calculation to become negative, while a wraparound results in a small (positive) number.

This can cause further issues. If, for example, the result is then used in an allocation, it will cause a runtime panic if it is negative, and allocate an unexpectedly small buffer otherwise.

Signed-off-by: Bhaskar <ram@hacker.ind.in>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 16:13:06 +0000 UTC
    </div>
</div>

