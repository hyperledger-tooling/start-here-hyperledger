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
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Bump private-data-objects from `5fa37a1` to `da7fddb`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [private-data-objects](https://github.com/hyperledger-labs/private-data-objects) from `5fa37a1` to `da7fddb`.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/da7fddba217ea7ac097e50c62b38f20e9520e2e1"><code>da7fddb</code></a> Move to standard tools for in-memory contract object cache</li>
<li>See full diff in <a href="https://github.com/hyperledger-labs/private-data-objects/compare/5fa37a13fac2749b1a6a43039ed2bee16d6cc70e...da7fddba217ea7ac097e50c62b38f20e9520e2e1">compare view</a></li>
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
        Created At 2024-05-10 01:30:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Add multi-issuer support for wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements a multi-issuer wallet. That is, a wallet that can manage (and perform operations on) assets from multiple issuers.  The wallet implements several widgets that can be used to import new issuers, check on the balance of holdings at multiple issuers (each with a unique identity), and transfer assets to other holdings (including identities with only a public key available, meaning other users running in other isolated containers).

The PR documents (or updates) three different test scenarios for the wallet:
* 06.single_user_wallet -- simple single issuer test
* 07.multiple_issuer_wallet -- test with a single wallet including multiple issuers
* 08.multier_user_wallet -- test with multiple wallets each with multiple issuers

Note that this PR does not include explicit contract flush at this point in time. That means that when refreshing the balance, it may require up to 30 seconds for the contract state to flush and be refreshed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-09 22:52:51 +0000 UTC
    </div>
</div>

