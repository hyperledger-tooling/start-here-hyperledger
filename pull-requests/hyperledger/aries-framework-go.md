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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3414" class=".btn">#3414</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/upload-artifact from 2.2.4 to 3.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 2.2.4 to 3.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v3.1.1</h2>
<ul>
<li>Update actions/core package to latest version to remove <code>set-output</code> deprecation warning <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/351">#351</a></li>
</ul>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​actions/artifact</code> to v1.1.0 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/pull/327">actions/upload-artifact#327</a>)
<ul>
<li>Adds checksum headers on artifact upload (<a href="https://github-redirect.dependabot.com/actions/toolkit/pull/1095">actions/toolkit#1095</a>) (<a href="https://github-redirect.dependabot.com/actions/toolkit/pull/1063">actions/toolkit#1063</a>)</li>
</ul>
</li>
</ul>
<h2>v3.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node16 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/293">#293</a>)</li>
<li>Update package-lock.json file version to 2 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/302">#302</a>)</li>
</ul>
<h3>Breaking Changes</h3>
<p>With the update to Node 16, all scripts will now be run with Node 16 rather than Node 12.</p>
<h2>v2.3.1</h2>
<p>Fix for empty fails on Windows failing on upload <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/281">#281</a></p>
<h2>v2.3.0 Upload Artifact</h2>
<ul>
<li>Optimizations for faster uploads of larger files that are already compressed</li>
<li>Significantly improved logging when there are chunked uploads</li>
<li>Clarifications in logs around the upload size and prohibited characters that aren't allowed in the artifact name or any uploaded files</li>
<li>Various other small bugfixes &amp; optimizations</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/83fd05a356d7e2593de66fc9913b3002723633cb"><code>83fd05a</code></a> Bump actions-core to v1.10.0 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/356">#356</a>)</li>
<li><a href="https://github.com/actions/upload-artifact/commit/3cea5372237819ed00197afe530f5a7ea3e805c8"><code>3cea537</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/327">#327</a> from actions/robherley/artifact-1.1.0</li>
<li><a href="https://github.com/actions/upload-artifact/commit/849aa7758a428ee22be38de371b49c8bd57c4b9d"><code>849aa77</code></a> nvm use 12 &amp; npm run release</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4d3986961d0423ba9a593efb490a2960eb65f43b"><code>4d39869</code></a> recompile with correct ncc version</li>
<li><a href="https://github.com/actions/upload-artifact/commit/2e0d362ec5cf81e334dda822c49c96dcd4b7df2c"><code>2e0d362</code></a> bump <code>@​actions/artifact</code> to 1.1.0</li>
<li><a href="https://github.com/actions/upload-artifact/commit/09a5d6a283da3e7c9f3253a5d4cdab2347712a66"><code>09a5d6a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/320">#320</a> from actions/dependabot/npm_and_yarn/ansi-regex-4.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/189315d9106f43a2a8eb60836608bb96b1f69d77"><code>189315d</code></a> Bump ansi-regex from 4.1.0 to 4.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d159c2d80bf32e77611286e4d71bfe6d15208d88"><code>d159c2d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/297">#297</a> from actions/dependabot/npm_and_yarn/ajv-6.12.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/c26a7ba4b5dbaecea906fec3b7d2c0c86f1ccaba"><code>c26a7ba</code></a> Bump ajv from 6.11.0 to 6.12.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/6ed6c729229a623bcb1fdd75903dc6e436b3d0a7"><code>6ed6c72</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/303">#303</a> from actions/dependabot/npm_and_yarn/yargs-parser-13.1.2</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v2.2.4...v3.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/upload-artifact&package-manager=github_actions&previous-version=2.2.4&new-version=3.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-24 08:19:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3413" class=".btn">#3413</a>
            </td>
            <td>
                <b>
                    feat: Update Tink version, protobuf type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the Tink version and our methods to use the newer protobuf type that it uses.

Reason for this change: the existing version of Tink makes use of a very large int in one particular place in the code, and this very large int prevents the gomobile tool from successfully generating Android bindings. This meant that aries-framework-go packages that used Tink could not be used in any code that you may want to generate Android bindings for. The updated version of Tink does not have that check anymore, which resolves the issue.

Due to a circular dependency between the main module and component/storage/edv (and the fact that both of them require Tink), there are some module/build issues with this commit. This will be resolved in the next commit.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 21:46:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3412" class=".btn">#3412</a>
            </td>
            <td>
                <b>
                    chore: add issuedAt claim to jwt
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
        Created At 2022-10-21 15:34:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3411" class=".btn">#3411</a>
            </td>
            <td>
                <b>
                    feat: support secp256k1 curve in KMS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds secp256k1 keys support in the kms for the IEEE-P1363 format only.
DER format is not supported because the x509 package does not support this curve.
The framework does support the creation of an secp256k1 key with DER format, however storing it in the KMS is not supported.

closes #3410

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 13:41:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3409" class=".btn">#3409</a>
            </td>
            <td>
                <b>
                    fix: parse generic ServicePoint
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
        Created At 2022-10-20 08:02:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3405" class=".btn">#3405</a>
            </td>
            <td>
                <b>
                    chore: handle PathNested in presexch
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
        Created At 2022-10-17 18:36:50 +0000 UTC
    </div>
</div>

