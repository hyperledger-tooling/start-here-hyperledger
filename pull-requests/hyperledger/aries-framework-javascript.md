---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1258" class=".btn">#1258</a>
            </td>
            <td>
                <b>
                    build(deps): bump http-cache-semantics from 4.1.0 to 4.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [http-cache-semantics](https://github.com/kornelski/http-cache-semantics) from 4.1.0 to 4.1.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/kornelski/http-cache-semantics/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=http-cache-semantics&package-manager=npm_and_yarn&previous-version=4.1.0&new-version=4.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 15:24:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1253" class=".btn">#1253</a>
            </td>
            <td>
                <b>
                    feat(indy-vdr): resolver and registrar for did:indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                An initial implementation of a resolver and registrar compliant with [did:indy](https://hyperledger.github.io/indy-did-method).

`IndyVdrIndyDidResolver` expects a full did:indy as an input and attempts to get it from the pools configured in IndyVdrPoolService. If the NYM is found, first attempts to build the DID Document combining the did/verkey and the `diddocContent`. If no diddocContent is received, it falls back to the good-old ATTRIB endpoint and reconstructs the DID Document using it.

`IndyVdrDidRegistrar` is a bit more flexible in terms of interface (TBD, by D meaning 'defined' and/or 'discussed'), as it can receive:
- a full did and a matching verkey; or
- a seed; or
- none of them

So in the first case it's assumed that the Key pair has been already created in the wallet and/or it is not needed to do so (e.g. we are anchoring a DID for someone else). In the other cases, the verkey is created and a matching did is dynamically generated.

In addition, in the options we can specify an array of `DidDocumentService` that will be added into the `diddocContent` on the NYM request, unless the user sets the flag `useEndpointAttrib`, which can be used for legacy deployments that don't support the didDocContent.

Some notes:

- There will be probably some other options for setting the version in NYM request (not yet supported by indy-vdr).
- DID Update and Deactivate are not yet implemented.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 02:59:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1252" class=".btn">#1252</a>
            </td>
            <td>
                <b>
                    feat(indy-vdr): use @hyperledger packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Waiting for the release of 0.1.0-dev.4 (https://github.com/hyperledger/indy-vdr/pull/150) for response type fixing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 21:11:38 +0000 UTC
    </div>
</div>

