---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/509" class=".btn">#509</a>
            </td>
            <td>
                <b>
                    Fix: publishing rev-reg should update value of handle, not create new
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 12:16:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/506" class=".btn">#506</a>
            </td>
            <td>
                <b>
                    Bump openssl-src from 111.17.0+1.1.1m to 111.22.0+1.1.1q
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl-src](https://github.com/alexcrichton/openssl-src-rs) from 111.17.0+1.1.1m to 111.22.0+1.1.1q.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/alexcrichton/openssl-src-rs/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl-src&package-manager=cargo&previous-version=111.17.0+1.1.1m&new-version=111.22.0+1.1.1q)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 20:11:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/505" class=".btn">#505</a>
            </td>
            <td>
                <b>
                    Remove old issuance APIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removed old libvcx approach to credential definitions and revocation registries, where these were tightly coupled together. Also removed respective node wrapper functions. 

```
vcx_credentialdef_create_and_store    | createAndStore
vcx_credentialdef_rotate_rev_reg_def  | rotateRevRegDef
vcx_credentialdef_publish_revocations | publishRevocations
vcx_credentialdef_get_tails_hash      | getTailsHash
vcx_credentialdef_get_rev_reg_id      | getRevRegId

vcx_revocation_registry_rotate        | rotate

vcx_issuer_send_credential_offer      | sendOffer
vcx_issuer_build_credential_offer_msg | was removed
```

- Apart from removing the interface, updated `libvcx` tests to follow the new approach, creating and publishing credential definitions and revocation registries independently.
- Few tests were deleted as they didn't no longer make sense or were not worth the effort
- Additionally packed in 1 bugfix: Function `revocation_registry::publish` was creating new revocation registry handle, instead of updating value of the existing one.


Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 14:02:08 +0000 UTC
    </div>
</div>

