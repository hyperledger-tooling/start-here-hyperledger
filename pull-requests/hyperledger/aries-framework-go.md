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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2993" class=".btn">#2993</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): bump clean-webpack-plugin from 3.0.0 to 4.0.0 in /cmd/aries-js-worker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [clean-webpack-plugin](https://github.com/johnagan/clean-webpack-plugin) from 3.0.0 to 4.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/johnagan/clean-webpack-plugin/releases">clean-webpack-plugin's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<p>Changes</p>
<ul>
<li>Added support for NodeJS 14</li>
<li>Added support for webpack 5</li>
</ul>
<p>Breaking changes:</p>
<ul>
<li>Dropped support for NodeJS 8</li>
<li>Dropped support for webpack 3</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/0207fe42de3da90c30ad492fd1dbe042dec2623b"><code>0207fe4</code></a> moved out of alpha, closes <a href="https://github-redirect.dependabot.com/johnagan/clean-webpack-plugin/issues/199">#199</a></li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/8190568b36987e901744d9656f6cefa041d18f5a"><code>8190568</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/johnagan/clean-webpack-plugin/issues/195">#195</a> from strootje/update-webpack-v5</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/6d8a2323a4700f2e01614c8606d1ed26853a63ce"><code>6d8a232</code></a> updated readme, cleaned up code as per PR suggestions</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/a164c19d1a24aba38872e7b56141c7dab419ecac"><code>a164c19</code></a> Merge branch 'master' into update-webpack-v5</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/c0749f539df37d8cdb730b39bab3f5cbd836e321"><code>c0749f5</code></a> updated code to not be to strictly typed, webpack fixed their types</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/f43ed055eef03dc26fe9839c216000f67e4fee5e"><code>f43ed05</code></a> Removed <code>@​types/webpack</code> dependency. This breaks with webpack 5</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/12649d84b8a262b69b0b2cf25a20cb257931d20e"><code>12649d8</code></a> fixed lint issue</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/4f7317a2074b1cc9a6f48392cda6609c855b9e25"><code>4f7317a</code></a> refactored code to match styling more, updated webpack typings</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/b2dccbbcd626a151772332ec1ba567473458a8c2"><code>b2dccbb</code></a> updated tests to match</li>
<li><a href="https://github.com/johnagan/clean-webpack-plugin/commit/0edf40f773d0868da2f7822beaec5dbb2611146d"><code>0edf40f</code></a> peerdependency correction</li>
<li>Additional commits viewable in <a href="https://github.com/johnagan/clean-webpack-plugin/compare/v3.0.0...v4.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=clean-webpack-plugin&package-manager=npm_and_yarn&previous-version=3.0.0&new-version=4.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2021-09-21 08:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2992" class=".btn">#2992</a>
            </td>
            <td>
                <b>
                    fix: add interop support to new didexchange key handling
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
        Created At 2021-09-21 00:16:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2991" class=".btn">#2991</a>
            </td>
            <td>
                <b>
                    chore: increase coverage for verifiable command fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 13:59:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2988" class=".btn">#2988</a>
            </td>
            <td>
                <b>
                    fix: verifiable command building KID from didDoc.VM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when didDoc.VM.ID has a #key-X suffix, the kms KID must be built from the VM.Value or VM.JWK() instead of being extracted from VM.ID

Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 15:26:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2987" class=".btn">#2987</a>
            </td>
            <td>
                <b>
                    feat: extend support cases for VC BBS derivation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - support embedded contexts: include custom contexts in bbs limited credential template
- support ID being optional: allow json-ld Processor to Frame docs with blank ID

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 06:33:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2986" class=".btn">#2986</a>
            </td>
            <td>
                <b>
                    chore: complete release 0.1.7
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
        Created At 2021-09-14 20:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    chore: Release 0.1.7
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
        Created At 2021-09-14 19:05:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2984" class=".btn">#2984</a>
            </td>
            <td>
                <b>
                    feat: add mediatype profiles and key types to agent-rest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 18:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/2983" class=".btn">#2983</a>
            </td>
            <td>
                <b>
                    feat: Present proof v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrii Soluk <isoluchok@gmail.com>
Signed-off-by: Baha Shaaban <baha.shaaban@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 17:56:14 +0000 UTC
    </div>
</div>

