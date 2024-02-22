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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2810" class=".btn">#2810</a>
            </td>
            <td>
                <b>
                    More updates to get docs publishing
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
        Created At 2024-02-22 14:56:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2806" class=".btn">#2806</a>
            </td>
            <td>
                <b>
                    Publish docs GHActions tweak
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
        Created At 2024-02-21 22:06:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2805" class=".btn">#2805</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump cryptography from 42.0.3 to 42.0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.3 to 42.0.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.4 - 2024-02-20</p>
<pre><code>
* Fixed a null-pointer-dereference and segfault that could occur when creating
  a PKCS#12 bundle. Credit to **Alexander-Programming** for reporting the
  issue. **CVE-2024-26130**
* Fixed ASN.1 encoding for PKCS7/SMIME signed messages. The fields ``SMIMECapabilities``
  and ``SignatureAlgorithmIdentifier`` should now be correctly encoded according to the
  definitions in :rfc:`2633` :rfc:`3370`.
<p>.. _v42-0-3:
</code></pre></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/fe18470f7d05f963e7267e34fdf985d81ea6ceea"><code>fe18470</code></a> Bump for 42.0.4 release (<a href="https://redirect.github.com/pyca/cryptography/issues/10445">#10445</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/aaa2dd06ed470695de818405a982d4c459869803"><code>aaa2dd0</code></a> Fix ASN.1 issues in PKCS#7 and S/MIME signing (<a href="https://redirect.github.com/pyca/cryptography/issues/10373">#10373</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10442">#10442</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/7a4d012991061974da5d9cb7614de65eac94f49b"><code>7a4d012</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10422">#10422</a> -- don't crash when a PKCS#12 key and cert don't match (<a href="https://redirect.github.com/pyca/cryptography/issues/10423">#10423</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/df314bb182bdfd661333969a94325e4680d785f6"><code>df314bb</code></a> backport actions m1 switch to 42.0.x (<a href="https://redirect.github.com/pyca/cryptography/issues/10415">#10415</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.3...42.0.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.3&new-version=42.0.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-02-21 20:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2804" class=".btn">#2804</a>
            </td>
            <td>
                <b>
                    Update publish-docs to operate on main and on branches prefixed with docs-v
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
        Created At 2024-02-21 18:53:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2803" class=".btn">#2803</a>
            </td>
            <td>
                <b>
                    Get and create anoncreds profile when using anoncreds subwallet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix https://github.com/hyperledger/aries-cloudagent-python/issues/2792, unless there's something I'm not aware of. 

Start the multitenant admin with
``` yml
wallet-type: askar-anoncreds
multitenancy-config: wallet_type=askar-profile
wallet-storage-type: default
```
and create tenant with 

``` json
{
  "extra_settings": {},
  "key_management_mode": "managed",
  "label": "Tenant 0",
  "wallet_dispatch_type": "default",
  "wallet_key": "tenant_key_0",
  "wallet_name": "tenant_0",
  "wallet_type": "askar-anoncreds"
}
```

Can create the ledger objects through the api. Before the change was get wrong profile error.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 21:30:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2802" class=".btn">#2802</a>
            </td>
            <td>
                <b>
                    Add index.html redirector to gh-pages branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 20:54:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2801" class=".btn">#2801</a>
            </td>
            <td>
                <b>
                    Add anoncreds multitenant endorsement integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                So, I had a misunderstanding. Endorsement for anoncreds in multitenancy is currently working when the admin agent is askar-anoncreds wallet type and the tenants are created with askar-anoncreds wallet type.

This PR will just add integration tests for this scenario.

I think it's important to have the feature https://github.com/hyperledger/aries-cloudagent-python/issues/2786 available for multitenancy going forward as this is where some of my confusion came from. When I first thought this didn't work, the author tenant wasn't setup completely. (It's pretty much finished other than some unit testing problems)

The other issue somewhat related to this issue is https://github.com/hyperledger/aries-cloudagent-python/issues/2792 but work can be done off of this issue as it is more relevant.

I'm thinking about how this is going to work with the admin agent on `askar` and a tenant is on `askar-anoncreds` and vice versa, and how this is going to work with the upgrade script etc. Currently this doesn't work because the wallet type of the admin agent is what decides what endpoints are available.

I don't think these questions are related to this ticket though so the tests should be enough to close this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 18:11:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2800" class=".btn">#2800</a>
            </td>
            <td>
                <b>
                    0.12.0rc1-tweak
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix to the publish GitHub action before release.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 14:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2799" class=".btn">#2799</a>
            </td>
            <td>
                <b>
                    0.12.0rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Draft still, as I would like to get a few more of the PRs in that are ready and just need merging.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-17 00:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2796" class=".btn">#2796</a>
            </td>
            <td>
                <b>
                    Change middleware registration order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This addresses issue #2666. The validation middlewares were registered before the authorization middlewares resulting in unauthorized requests executing the validation code in the application. This leads to a security flaw as validation libraries could be exploited and could be considered a form [remote code injection](https://owasp.org/www-community/attacks/Code_Injection).

The fix is simple and results on authorization checks happening before request validations. 

@esune @amanji please review these changes and let me know what you think!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 23:49:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2795" class=".btn">#2795</a>
            </td>
            <td>
                <b>
                    Bump pyld version to 2.0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to address a bug we have found in the pyld library which was incorrectly asserting context elements as null.

Addresses issue #2743 and will close PR #2744.

For background information you can read [this closed issue on the pyld repo](https://github.com/digitalbazaar/pyld/pull/189).

@swcurran I tested these changes and was able to verify traceable credentials with the proper did document content. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 23:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2794" class=".btn">#2794</a>
            </td>
            <td>
                <b>
                    Revert profile injection for VcLdpManager on vc-api endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pretty straightforward, I changed the way these endpoint instantiate the `VcLdpManager`. This is to address [this issue](https://github.com/hyperledger/aries-cloudagent-python/issues/2793)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 22:07:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2791" class=".btn">#2791</a>
            </td>
            <td>
                <b>
                    Author subwallet setup automation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows tenant author setup with an endorser to be automated through the api with the same configs as starting an author agent from the command line. It creates a util with the existing startup code and calls it from the `create_wallet` endpoint. I think this really helps simplify creating author tenants.

example:
``` json
{
  "extra_settings": {
    "endorser-alias": "endorser",
    "endorser-protocol-role": "author",
    "auto-request-endorsement": true,
    "auto-write-transactions": true,
    "endorser-public-did": "Aedt1jccq9Do7G9fKp7yHT",
    "auto-promote-author-did": true,
    "auto-create-revocation-transactions": true,
    "endorser-invitation": "http://localhost:9030?oob=eyJAdHlwZSI6ICJodHRwczovL2RpZGNvbW0ub3JnL291dC1vZi1iYW5kLzEuMS9pbnZpdGF0aW9uIiwgIkBpZCI6ICIxZTEyZjY0ZC05MWYwLTRlM2YtYmZmMi1jYzk5NjkxMDNhOWMiLCAibGFiZWwiOiAiZW5kb3JzZXIiLCAiaGFuZHNoYWtlX3Byb3RvY29scyI6IFsiaHR0cHM6Ly9kaWRjb21tLm9yZy9kaWRleGNoYW5nZS8xLjAiXSwgInNlcnZpY2VzIjogW3siaWQiOiAiI2lubGluZSIsICJ0eXBlIjogImRpZC1jb21tdW5pY2F0aW9uIiwgInJlY2lwaWVudEtleXMiOiBbImRpZDprZXk6ejZNa3RFajlkdFJ3UXFzRllWUGpTeEZKYlJHZkN2emExUWoxcU5USjE3TWFza1RqI3o2TWt0RWo5ZHRSd1Fxc0ZZVlBqU3hGSmJSR2ZDdnphMVFqMXFOVEoxN01hc2tUaiJdLCAic2VydmljZUVuZHBvaW50IjogImh0dHA6Ly9sb2NhbGhvc3Q6OTAzMCJ9XX0="
  },
  "key_management_mode": "managed",
  "label": "tenant-0",
  "wallet_dispatch_type": "default",
  "wallet_key": "tenant-key-0",
  "wallet_name": "tenant-0",
  "wallet_type": "askar-anoncreds"
}
```

I had to fix what I believe was a bug with creating the connection for the tenant from the admin context in `aries_cloudagent/protocols/didexchange/v1_0/manager.py` where connection info would be saved for the wrong profile for the responder.


 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 17:43:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2790" class=".btn">#2790</a>
            </td>
            <td>
                <b>
                    feature/per tenant settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Adds `--emit-did-peer-{2 | 4}` per tenant setting
- Adds `--preserve-exchange-records` per tenant setting
- Adds  `--requests-through-public-did` per tenant setting

Resolves: #2724 
Resolves: #2648
Resolves: #2572 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 17:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2789" class=".btn">#2789</a>
            </td>
            <td>
                <b>
                    Revert profile inject
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts the changes made in https://github.com/hyperledger/aries-cloudagent-python/pull/2705 which caused problems with certain multitenant environments (still unknown). If this is something we want we can look at doing it again in a future release.

Tested the problem described in issue https://github.com/hyperledger/aries-cloudagent-python/issues/2777 by running the multitenant provider plugin integration tests. Could see the problem in 0.12.0dev0, but all the tests pass when pointing to my forked branch with the revert.

I believe this was only used for the `VcLdpManager` to prevent creating a new instance for every handler method call. I reverted these occurrences back to creating a new manager instance. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 21:29:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2788" class=".btn">#2788</a>
            </td>
            <td>
                <b>
                    Add known issues section to Multiledger.md documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a note to the multiledger documentation that references a known issue when switching ledgers.

@dbluhm @swcurran I referenced the open issue, but didn't add additional details as they will likely be documented in the issue itself.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 19:59:24 +0000 UTC
    </div>
</div>

