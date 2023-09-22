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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2503" class=".btn">#2503</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 41.0.3 to 41.0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 41.0.3 to 41.0.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.4 - 2023-09-19</p>
<pre><code>
* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.3.
<p>.. _v41-0-3:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/fc11bce6930e591ce26a2317b31b9ce2b3e25512"><code>fc11bce</code></a> bump for 41.0.4 (<a href="https://redirect.github.com/pyca/cryptography/issues/9629">#9629</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/41.0.3...41.0.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=41.0.3&new-version=41.0.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-09-21 21:30:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2502" class=".btn">#2502</a>
            </td>
            <td>
                <b>
                    fix: mediation webhook routing keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Re: #[2357](https://github.com/hyperledger/aries-cloudagent-python/issues/2357) and #[2492](https://github.com/hyperledger/aries-cloudagent-python/issues/2492)

Indicio PR: https://github.com/Indicio-tech/aries-cloudagent-python/pull/153

Tagging and credit due to @dbluhm 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 19:00:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2500" class=".btn">#2500</a>
            </td>
            <td>
                <b>
                    fix: update pydid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will correct the errror reported in #2497.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 16:37:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2499" class=".btn">#2499</a>
            </td>
            <td>
                <b>
                    Use correct rust log level in dockerfiles 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                From issue https://github.com/hyperledger/aries-cloudagent-python/issues/2498

It looks like `warning` is not a valid Rust log level string https://docs.rs/log/latest/log/enum.Level.html
From what I've seen in traction (which deploys using the dockerfile here), this means logs default to INFO level here even though dockerfile is trying to have it at the warn level. (see details in ticket for what I tried out)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-21 04:12:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2496" class=".btn">#2496</a>
            </td>
            <td>
                <b>
                    Fix: Ledger error when registering nym after multi-ledger switch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2473 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-19 16:14:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2495" class=".btn">#2495</a>
            </td>
            <td>
                <b>
                    fix: run tests script copying local env
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the scripts/run_tests script and its dockerfiles to make sure it doesn't copy local .venv directories into the container image. This was causing the script to fail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 18:53:16 +0000 UTC
    </div>
</div>

