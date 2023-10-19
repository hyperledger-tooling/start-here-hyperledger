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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2557" class=".btn">#2557</a>
            </td>
            <td>
                <b>
                    [Snyk] Security upgrade urllib3 from 2.0.6 to 2.0.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <p>This PR was automatically created by Snyk using the credentials of a real user.</p><br /><h3>Snyk has created this PR to fix one or more vulnerable packages in the `pip` dependencies of this project.</h3>



#### Changes included in this PR

- Changes to the following files to upgrade the vulnerable dependencies to a fixed version:
    - demo/playground/scripts/requirements.txt



#### Vulnerabilities that will be fixed





##### By pinning:
Severity                   | Priority Score (*)                   | Issue                   | Upgrade                   | Breaking Change                   | Exploit Maturity
:-------------------------:|-------------------------|:-------------------------|:-------------------------|:-------------------------|:-------------------------
![medium severity](https://res.cloudinary.com/snyk/image/upload/w_20,h_20/v1561977819/icon/m.png "medium severity")  |  **496/1000**  <br/> **Why?** Recently disclosed, Has a fix available, CVSS 4.2  | Information Exposure Through Sent Data <br/>[SNYK-PYTHON-URLLIB3-6002459](https://snyk.io/vuln/SNYK-PYTHON-URLLIB3-6002459) |  `urllib3:` <br> `2.0.6 -> 2.0.7` <br>  |  No  | No Known Exploit 

(*) Note that the real score may have changed since the PR was raised.




Some vulnerabilities couldn't be fully fixed and so Snyk will still find them when the project is tested again. This may be because the vulnerability existed within more than one direct dependency, but not all of the affected dependencies could be upgraded.


Check the changes in this PR to ensure they won't cause issues with your project.



------------



**Note:** *You are seeing this because you or someone else with access to this repository has authorized Snyk to open fix PRs.*

For more information:  <img src="https://api.segment.io/v1/pixel/track?data=eyJ3cml0ZUtleSI6InJyWmxZcEdHY2RyTHZsb0lYd0dUcVg4WkFRTnNCOUEwIiwiYW5vbnltb3VzSWQiOiIwZjk0ZmVhNi0xZjI4LTQwODQtODU3NC01NWIwMTNlNzI4MDYiLCJldmVudCI6IlBSIHZpZXdlZCIsInByb3BlcnRpZXMiOnsicHJJZCI6IjBmOTRmZWE2LTFmMjgtNDA4NC04NTc0LTU1YjAxM2U3MjgwNiJ9fQ==" width="0" height="0"/>
🧐 [View latest project report](https://app.snyk.io/org/hyperledger-bot/project/91e9cfad-3cfa-4801-bdbf-fa8afcd5c91d?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;fix-pr)

🛠 [Adjust project settings](https://app.snyk.io/org/hyperledger-bot/project/91e9cfad-3cfa-4801-bdbf-fa8afcd5c91d?utm_source&#x3D;github&amp;utm_medium&#x3D;referral&amp;page&#x3D;fix-pr/settings)

📚 [Read more about Snyk's upgrade and patch logic](https://support.snyk.io/hc/en-us/articles/360003891078-Snyk-patches-to-fix-vulnerabilities)

[//]: # (snyk:metadata:{"prId":"0f94fea6-1f28-4084-8574-55b013e72806","prPublicId":"0f94fea6-1f28-4084-8574-55b013e72806","dependencies":[{"name":"urllib3","from":"2.0.6","to":"2.0.7"}],"packageManager":"pip","projectPublicId":"91e9cfad-3cfa-4801-bdbf-fa8afcd5c91d","projectUrl":"https://app.snyk.io/org/hyperledger-bot/project/91e9cfad-3cfa-4801-bdbf-fa8afcd5c91d?utm_source=github&utm_medium=referral&page=fix-pr","type":"auto","patch":[],"vulns":["SNYK-PYTHON-URLLIB3-6002459"],"upgrade":[],"isBreakingChange":false,"env":"prod","prType":"fix","templateVariants":["updated-fix-title","priorityScore"],"priorityScoreList":[496],"remediationStrategy":"vuln"})

---

**Learn how to fix vulnerabilities with free interactive lessons:**

 🦉 [Learn about vulnerability in an interactive lesson of Snyk Learn.](https://learn.snyk.io/?loc&#x3D;fix-pr)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-19 05:38:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2554" class=".btn">#2554</a>
            </td>
            <td>
                <b>
                    fix: taa rough timestamp timezone from datetime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2553
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 18:10:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2552" class=".btn">#2552</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.0.6 to 2.0.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 2.0.6 to 2.0.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.0.7</h2>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses. (GHSA-g4mx-q9vg-27p4)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.0.7 (2023-10-17)</h1>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/56f01e088dc006c03d4ee6ea9da4ab810f1ed700"><code>56f01e0</code></a> Release 2.0.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/4e50fbc5db74e32cabd5ccc1ab81fc103adfe0b3"><code>4e50fbc</code></a> Merge pull request from GHSA-g4mx-q9vg-27p4</li>
<li><a href="https://github.com/urllib3/urllib3/commit/80808b04bfa68fbd099828848c96ee25df185f1d"><code>80808b0</code></a> Fix docs build on Python 3.12 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3144">#3144</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f28deff1cf162c673b50d88d3552e91bda6d68a8"><code>f28deff</code></a> Add 1.26.17 to the current changelog</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/2.0.6...2.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.0.6&new-version=2.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-17 21:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2551" class=".btn">#2551</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump urllib3 from 2.0.6 to 2.0.7 in /demo/playground/scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 2.0.6 to 2.0.7.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>2.0.7</h2>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses. (GHSA-g4mx-q9vg-27p4)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>2.0.7 (2023-10-17)</h1>
<ul>
<li>Made body stripped from HTTP requests changing the request method to GET after HTTP 303 &quot;See Other&quot; redirect responses.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/56f01e088dc006c03d4ee6ea9da4ab810f1ed700"><code>56f01e0</code></a> Release 2.0.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/4e50fbc5db74e32cabd5ccc1ab81fc103adfe0b3"><code>4e50fbc</code></a> Merge pull request from GHSA-g4mx-q9vg-27p4</li>
<li><a href="https://github.com/urllib3/urllib3/commit/80808b04bfa68fbd099828848c96ee25df185f1d"><code>80808b0</code></a> Fix docs build on Python 3.12 (<a href="https://redirect.github.com/urllib3/urllib3/issues/3144">#3144</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/f28deff1cf162c673b50d88d3552e91bda6d68a8"><code>f28deff</code></a> Add 1.26.17 to the current changelog</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/2.0.6...2.0.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=2.0.6&new-version=2.0.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-17 21:03:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2550" class=".btn">#2550</a>
            </td>
            <td>
                <b>
                    Feat: Per Tenant Logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2359 
- Derived from work done in #2425 
- Needed to close that PR as the pre-release images in there somehow included legacy code which was removed subsequently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 13:58:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2548" class=".btn">#2548</a>
            </td>
            <td>
                <b>
                    Update .readthedocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Another fix to this YAML file. Unfortunately, I can't test it without getting it into main (AFAIK...).  Frustrating...

Errors were dumb in the last try...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-15 20:16:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2547" class=".btn">#2547</a>
            </td>
            <td>
                <b>
                    Update .readthedocs.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RTD is broken because (I think) missing section of RTD.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-14 22:56:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2546" class=".btn">#2546</a>
            </td>
            <td>
                <b>
                    DRAFT: please_ack support PoC for the 0453-issue-credential-v2 protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is PoC code for the PR#2540 (https://github.com/hyperledger/aries-cloudagent-python/pull/2540). It shows possible implementation of the `please_ack` decorator support ('option 2' in the document in the PR#2540)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 11:23:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2545" class=".btn">#2545</a>
            </td>
            <td>
                <b>
                    :art: clarify LedgerError message when TAA is required and not accepted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously:
```py
            if await self.is_ledger_read_only():
                raise LedgerError(
                    "Error cannot write cred def when ledger is in read only mode"
                )
```

`is_ledger_read_only` also checks to see if TAA is required, and if not accepted it will also report the ledger is read-only:
```py
    async def is_ledger_read_only(self) -> bool:
        """Check if ledger is read-only including TAA."""
        if self.read_only:
            return self.read_only
        # if TAA is required and not accepted we should be in read-only mode
        taa = await self.get_txn_author_agreement()
        if taa["taa_required"]:
            taa_acceptance = await self.get_latest_txn_author_acceptance()
            if "mechanism" not in taa_acceptance:
                return True
        return self.read_only
```

To make this clearer to the user, I updated the relevant error messages to say TAA  may also be the cause of the LedgerError.

e.g.:
```py
                raise LedgerError(
                    "Error cannot write cred def when ledger is in read only mode, "
                    "or TAA is required and not accepted"
                )
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 09:34:54 +0000 UTC
    </div>
</div>

