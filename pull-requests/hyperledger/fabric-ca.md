---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    Release commit for v1.5.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add release notes for v1.5.10.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 16:40:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    Bump idna from 3.6 to 3.7 in /docs
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric-ca/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 04:29:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    GO-2024-2687.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to Go v1.21.9 and x/net v0.23.0 to address GO-2024-2687.

See https://pkg.go.dev/vuln/GO-2024-2687
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 17:48:48 +0000 UTC
    </div>
</div>

