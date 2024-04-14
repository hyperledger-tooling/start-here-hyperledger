---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2892" class=".btn">#2892</a>
            </td>
            <td>
                <b>
                    feat: drop indy sdk
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.0.0</span>
            </td>
            <td>
                Resolves #2865

This is a quick pass at removing all imports of the Indy SDK. I'll spend some more time scanning for other spots where references to the indy wallet type are made (e.g. cli args).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-13 19:35:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2891" class=".btn">#2891</a>
            </td>
            <td>
                <b>
                    fix: look up conn record by invite msg id instead of key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2890.

When reusing DIDs in invitations, the invitation key is no longer a unique value by which a connection record can be discovered. To workaround this, this change causes connection records to be looked up by invitation message id (request message's pthid) instead of by invitation key.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-13 18:55:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2889" class=".btn">#2889</a>
            </td>
            <td>
                <b>
                    fix: integration tests should use didex 1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A quick fix for the integration tests. I added the `use_did_method` parameter to the `get_invite` method of the support agent class but forgot to update the `handshake_protocols` list used to did exchange 1.1. Without this change, the int tests were actually just defaulting back to 1.0 behavior of unqualified DIDs.

This is just a correction in the tests and does not impact the behavior of ACA-Py which, according to my own testing at least, is still correctly sending qualified DIDs in the appropriate circumstances.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 17:47:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2888" class=".btn">#2888</a>
            </td>
            <td>
                <b>
                    Some updates to the mkdocs publishing process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 14:43:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2887" class=".btn">#2887</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump idna from 3.6 to 3.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [idna](https://github.com/kjd/idna) from 3.6 to 3.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=idna&package-manager=pip&previous-version=3.6&new-version=3.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 04:05:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2886" class=".btn">#2886</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump idna from 3.4 to 3.7 in /demo/playground/examples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [idna](https://github.com/kjd/idna) from 3.4 to 3.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/releases">idna's releases</a>.</em></p>
<blockquote>
<h2>v3.7</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix issue where specially crafted inputs to encode() could take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p><strong>Full Changelog</strong>: <a href="https://github.com/kjd/idna/compare/v3.6...v3.7">https://github.com/kjd/idna/compare/v3.6...v3.7</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/kjd/idna/blob/master/HISTORY.rst">idna's changelog</a>.</em></p>
<blockquote>
<p>3.7 (2024-04-11)
++++++++++++++++</p>
<ul>
<li>Fix issue where specially crafted inputs to encode() could
take exceptionally long amount of time to process. [CVE-2024-3651]</li>
</ul>
<p>Thanks to Guido Vranken for reporting the issue.</p>
<p>3.6 (2023-11-25)
++++++++++++++++</p>
<ul>
<li>Fix regression to include tests in source distribution.</li>
</ul>
<p>3.5 (2023-11-24)
++++++++++++++++</p>
<ul>
<li>Update to Unicode 15.1.0</li>
<li>String codec name is now &quot;idna2008&quot; as overriding the system codec
&quot;idna&quot; was not working.</li>
<li>Fix typing error for codec encoding</li>
<li>&quot;setup.cfg&quot; has been added for this release due to some downstream
lack of adherence to PEP 517. Should be removed in a future release
so please prepare accordingly.</li>
<li>Removed reliance on a symlink for the &quot;idna-data&quot; tool to comport
with PEP 517 and the Python Packaging User Guide for sdist archives.</li>
<li>Added security reporting protocol for project</li>
</ul>
<p>Thanks Jon Ribbens, Diogo Teles Sant'Anna, Wu Tingfeng for contributions
to this release.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kjd/idna/commit/1d365e17e10d72d0b7876316fc7b9ca0eebdd38d"><code>1d365e1</code></a> Release v3.7</li>
<li><a href="https://github.com/kjd/idna/commit/c1b3154939907fab67c5754346afaebe165ce8e6"><code>c1b3154</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/172">#172</a> from kjd/optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/0394ec76ff022813e770ba1fd89658790ea35623"><code>0394ec7</code></a> Merge branch 'master' into optimize-contextj</li>
<li><a href="https://github.com/kjd/idna/commit/cd58a23173d2b0a40b95ee680baf3e59e8d33966"><code>cd58a23</code></a> Merge pull request <a href="https://redirect.github.com/kjd/idna/issues/152">#152</a> from elliotwutingfeng/dev</li>
<li><a href="https://github.com/kjd/idna/commit/5beb28b9dd77912c0dd656d8b0fdba3eb80222e7"><code>5beb28b</code></a> More efficient resolution of joiner contexts</li>
<li><a href="https://github.com/kjd/idna/commit/1b121483ed04d9576a1291758f537e1318cddc8b"><code>1b12148</code></a> Update ossf/scorecard-action to v2.3.1</li>
<li><a href="https://github.com/kjd/idna/commit/d516b874c3388047934938a500c7488d52c4e067"><code>d516b87</code></a> Update Github actions/checkout to v4</li>
<li><a href="https://github.com/kjd/idna/commit/c095c75943413c75ebf8ac74179757031b7f80b7"><code>c095c75</code></a> Merge branch 'master' into dev</li>
<li><a href="https://github.com/kjd/idna/commit/60a0a4cb61ec6834d74306bd8a1fa46daac94c98"><code>60a0a4c</code></a> Fix typo in GitHub Actions workflow key</li>
<li><a href="https://github.com/kjd/idna/commit/5918a0ef8034379c2e409ae93ee11d24295bb201"><code>5918a0e</code></a> Merge branch 'master' into dev</li>
<li>Additional commits viewable in <a href="https://github.com/kjd/idna/compare/v3.4...v3.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=idna&package-manager=pip&previous-version=3.4&new-version=3.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 03:19:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2885" class=".btn">#2885</a>
            </td>
            <td>
                <b>
                    Prevent 500 error when re-promoting DID with endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/aries-cloudagent-python/issues/2884

Just decided to fix this when I saw it. Doesn't cause any issues but prevents an unwanted 500 error.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 20:19:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2883" class=".btn">#2883</a>
            </td>
            <td>
                <b>
                    Fix ack during for auto endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevents the `TransactionManagerError` when doing endorsement ack without setting up jobs in auto_endorse mode.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 20:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2882" class=".btn">#2882</a>
            </td>
            <td>
                <b>
                    0.12.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 17:23:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2881" class=".btn">#2881</a>
            </td>
            <td>
                <b>
                    Add anoncreds migration guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a migration guide controllers to upgrade to anoncreds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 16:25:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2880" class=".btn">#2880</a>
            </td>
            <td>
                <b>
                    fix: conn proto in invite webhook if known
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2879. See the issue for details and reasoning.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 17:35:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2878" class=".btn">#2878</a>
            </td>
            <td>
                <b>
                    0.12.0rc3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Final (we hope) RC before the release.  Need to focus a little more on the content of the Changelog message. Doesn't have to be perfect on this one, but feedback definitely welcome on what we highlight, what we talk about, and what links to additional material we cover.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 21:49:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2877" class=".btn">#2877</a>
            </td>
            <td>
                <b>
                    Add wallet.type config to /settings endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/aries-cloudagent-python/issues/2876
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-08 16:02:55 +0000 UTC
    </div>
</div>

