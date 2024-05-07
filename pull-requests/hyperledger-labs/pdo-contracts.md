---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Jupyter support for multiple, independent users
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds Jupyter support for multiple independent users to share token and issuer contracts. 
First basic implementation of a wallet for a single issuer
Scenarios for testing (05 and 06 should work, 07 is future work)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 23:04:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Couple fixes that will make the multiuser tests easier to build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds two things:
* A multiuser jupyter test (basically just starts 3 containers each with separate jupyter instanced); allows for testing sharing of contracts between distinct users.
* Better support for moving files into and out of containers; file upload widget, contract import, key download.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 15:16:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Fix typo in new docker compose macro
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small PR to fix a typo in the last docker compose PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 16:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    Bump private-data-objects from `d5d94df` to `5fa37a1`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [private-data-objects](https://github.com/hyperledger-labs/private-data-objects) from `d5d94df` to `5fa37a1`.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/5fa37a13fac2749b1a6a43039ed2bee16d6cc70e"><code>5fa37a1</code></a> Adding comments to pdo tp and pservice code where enclave ias attestation ver...</li>
<li>See full diff in <a href="https://github.com/hyperledger-labs/private-data-objects/compare/d5d94df14eaae2ee4ebb68ccafb4e101dedfa27e...5fa37a13fac2749b1a6a43039ed2bee16d6cc70e">compare view</a></li>
</ul>
</details>
<br />


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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 01:40:53 +0000 UTC
    </div>
</div>

