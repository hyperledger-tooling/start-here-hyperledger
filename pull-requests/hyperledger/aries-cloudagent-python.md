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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2651" class=".btn">#2651</a>
            </td>
            <td>
                <b>
                    Update integration tests for anoncreds-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Opening in draft for visibility
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-04 18:55:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2645" class=".btn">#2645</a>
            </td>
            <td>
                <b>
                    feat: add did:jwk resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This implements a did:jwk resolver. See https://github.com/hyperledger/aries-acapy-plugins/pull/47 for context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 22:07:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2643" class=".btn">#2643</a>
            </td>
            <td>
                <b>
                    Initial migration of anoncreds revocation code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Adds revocation support from the anoncreds-rs branch.  Still a few TODO's but this PR is ready to go and I'll continue the work in the next PR.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 19:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2642" class=".btn">#2642</a>
            </td>
            <td>
                <b>
                    Feat: DIDX Implicit Request auto-accept and Delete OOB Invitation related records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #2644
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 16:57:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2638" class=".btn">#2638</a>
            </td>
            <td>
                <b>
                    fix: update broken demo dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Couldn't proceed with further local testing on my host. Probably due to differences in python versions. 

```
    self.proc = await asyncio.wait_for(future, 20, loop=loop)
                      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
TypeError: wait_for() got an unexpected keyword argument 'loop'
```

But pip install works fine now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 14:22:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2636" class=".btn">#2636</a>
            </td>
            <td>
                <b>
                    Bump cryptography from 41.0.5 to 41.0.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 41.0.5 to 41.0.6.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>41.0.6 - 2023-11-27</p>
<pre><code>
* Fixed a null-pointer-dereference and segfault that could occur when loading
  certificates from a PKCS#7 bundle.  Credit to **pkuzco** for reporting the
  issue. **CVE-2023-49083**
<p>.. _v41-0-5:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/f09c261ca10a31fe41b1262306db7f8f1da0e48a"><code>f09c261</code></a> 41.0.6 release (<a href="https://redirect.github.com/pyca/cryptography/issues/9927">#9927</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/41.0.5...41.0.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=41.0.5&new-version=41.0.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-29 00:26:16 +0000 UTC
    </div>
</div>

