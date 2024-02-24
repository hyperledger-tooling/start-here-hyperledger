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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2814" class=".btn">#2814</a>
            </td>
            <td>
                <b>
                    Fix anoncreds non-endorsement revocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sorry. I should have blocked the last PR from getting merged for a bit. I forgot to test the anoncreds non-endorsement scenario. Integration tests caught it and I fixed the problem with this PR. Tested the failing integration tests locally.

Also, enabled a test that was commented out for askar wallet revoke and then publish scenarios.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 22:51:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2813" class=".btn">#2813</a>
            </td>
            <td>
                <b>
                    Fix connection reuse handling in demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Separate the "connection reuse" and "use public did" configuration for the demo:

```
./run_demo faber --reuse-connection --public-did-connections
```

(Previously only the `--reuse-connection` parameter was available and it automatically set the connection to use the public DID.)

To run with a `did:peer` use:

```
DEMO_EXTRA_AGENT_ARGS="[\"--emit-did-peer-2\"]" ./run_demo faber --reuse-connection --events
```

There are some issues with `did:peer`, see discussion in issue #2703.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-23 18:56:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2812" class=".btn">#2812</a>
            </td>
            <td>
                <b>
                    Create revocation notification after list entry written to ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes the issue with the revocation notification not happening.

There was a couple things that didn't make sense. 

- For the `/revoke` endpoint if was never calling notify. It was only creating the notification record. This may have been deliberate (see comment), but needs to notify at some point, which it isn't doing.
- For the `/publish-revocations` endpoint it was not calling notify when there was a connection_id, but this is only used for explicitly using a specific endorser connection. When in author and preconfigured mode, this parameter isn't even used. I think it was trying to prevent the notify from happening for endorsement scenarios. (see next comment)

***comment***: right now the revocation notification is happening after requesting endorsement but before the new list entry has been written to the ledger. This is the same for anoncreds. I'm not sure if this is what we actually want. It kinda makes sense to have it immediately when the issuer revokes, but it also makes sense not to notify until after the endorsement has happened and the entry has been written.

Tested with traction and bc wallet. 

Still testing some scenarios.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 20:01:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2811" class=".btn">#2811</a>
            </td>
            <td>
                <b>
                    Eliminate the double workflow event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removes the "on create" trigger, since that seems to trigger the workflow twice.
Fixes the version of the variable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 19:31:47 +0000 UTC
    </div>
</div>

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

