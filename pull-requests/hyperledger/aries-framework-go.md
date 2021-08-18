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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2941" class=".btn">#2941</a>
            </td>
            <td>
                <b>
                    fix: set config for remote provider store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 14:45:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2940" class=".btn">#2940</a>
            </td>
            <td>
                <b>
                    fix: integration issues in wallet DIDcomm interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:34:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2938" class=".btn">#2938</a>
            </td>
            <td>
                <b>
                    docs: Updates to storage interface documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Clarified expected behaviour of storage interface implementations
- Added missing call to Provider.SetStoreConfig for the context store.
- Removed the workaround for MySQL, which is no longer needed.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:12:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2937" class=".btn">#2937</a>
            </td>
            <td>
                <b>
                    refactor: use did:key in packagers (for didcomm v1)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">refactor</span><span class="chip">aip 2.0</span>
            </td>
            <td>
                This change removes Base58 key encoding for recipients and sender for did:key (execept for legacy packer which will remain using bsae58 encoding).
It also includes vdr peer did creation with all VM and KeyAgreement keys, not only the first key.
This change adds key resolvers for the packers, one for did:key resolution and another one used for the 1PU test vector verification purposes using a thirdparty store resolution.
Finally, this change also moves did:key fingerprint code referencing did.Doc into a separate subpackage (pkg/vdr/fingerprint/didfp) to avoid cyclic dependency with jwk fingerprint.

closes #1604
closes #1207
closes #1659
closes #1847

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 18:17:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2936" class=".btn">#2936</a>
            </td>
            <td>
                <b>
                    fix: add close request
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
        Created At 2021-08-16 16:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2934" class=".btn">#2934</a>
            </td>
            <td>
                <b>
                    fix: context store Import when underlying storage is mysql
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 09:42:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2933" class=".btn">#2933</a>
            </td>
            <td>
                <b>
                    chore(deps): bump tar from 6.1.0 to 6.1.8 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [tar](https://github.com/npm/node-tar) from 6.1.0 to 6.1.8.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/npm/node-tar/commit/6a9c51da31a2c9b67d266d8ce7119e1e2c0d1e5d"><code>6a9c51d</code></a> 6.1.8</li>
<li><a href="https://github.com/npm/node-tar/commit/dfc5923b965aff780d0d8eb4dd657195ee095c41"><code>dfc5923</code></a> fix: skip extract if linkpath is stripped entirely</li>
<li><a href="https://github.com/npm/node-tar/commit/575a511cda6fe3ad201d8a576caaf30abea808a4"><code>575a511</code></a> fix: reserve paths case-insensitively</li>
<li><a href="https://github.com/npm/node-tar/commit/d61628cb40381d89f119431a16a4aab2fbecb056"><code>d61628c</code></a> 6.1.7</li>
<li><a href="https://github.com/npm/node-tar/commit/9e018cf2a5e289d6b34d1a0157980070b3a14c75"><code>9e018cf</code></a> tests: run (and pass) on windows</li>
<li><a href="https://github.com/npm/node-tar/commit/c2a0948fb7b70862f92828e7b37b622566ed367e"><code>c2a0948</code></a> fix: refactoring to pass tests on Windows</li>
<li><a href="https://github.com/npm/node-tar/commit/d0ce670bdb7eed5861837538a0d18c7864ff71c6"><code>d0ce670</code></a> update deps</li>
<li><a href="https://github.com/npm/node-tar/commit/53602669f58ddbeb3294d7196b3320aaaed22728"><code>5360266</code></a> fix: normalize paths on Windows systems</li>
<li><a href="https://github.com/npm/node-tar/commit/9bc1729939eec1c822b528385b1cc513b9888835"><code>9bc1729</code></a> 6.1.6</li>
<li><a href="https://github.com/npm/node-tar/commit/bdf4f5171340b890a62a5e578962ac143d34b3a9"><code>bdf4f51</code></a> fix: properly prefix hard links</li>
<li>Additional commits viewable in <a href="https://github.com/npm/node-tar/compare/v6.1.0...v6.1.8">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tar&package-manager=npm_and_yarn&previous-version=6.1.0&new-version=6.1.8)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-08-13 12:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2932" class=".btn">#2932</a>
            </td>
            <td>
                <b>
                    chore: Updated json-gold module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 12:03:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2931" class=".btn">#2931</a>
            </td>
            <td>
                <b>
                    docs: vcwallet didcomm interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added docs for connect, proposePresentation & presentProof interfaces
in vcwallet.
- part of #2433

Signed-off-by: sudesh.shetty <sudesh.shetty@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 16:17:13 +0000 UTC
    </div>
</div>

