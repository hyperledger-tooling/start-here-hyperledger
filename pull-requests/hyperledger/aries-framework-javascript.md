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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1550" class=".btn">#1550</a>
            </td>
            <td>
                <b>
                    feat: did:peer:2 support in DID Exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some initial work on supporting `did:peer:2` in DID Exchange protocol, in order to start aligning with [RFC 0793](https://github.com/hyperledger/aries-rfcs/blob/fcb2cafce6abea0995804c32a6da473c8894e470/features/0793-unqualfied-dids-transition/README.md).

Currently, AFJ uses qualified DIDs for DID Exchange protocol, in `did:peer:1` format. The community is going towards `did:peer:2` and the new `did:peer:3` (more meaningful in DIDComm v2 world). So in this PR we are trying to do the transition from `did:peer:1` to `did:peer:2` in order to be compatible with ACA-Py when it adds support for the reception of qualified DIDs in DID Exchange protocol.

At the moment, the logic is the following:
- There is a new setting in `ConnectionsModuleConfig` to choose the default DID Peer num algo to use in DID Exchange Requests. If not defined, did:peer:1 will be used (this is current behaviour)
- There is a new optional setting in both OOB Reception and Invitation acceptance methods to override default setting. The use case would be: we know our mediator supports only `did:peer:2` (ACA-Py) so we connect with it using that algo, while still using `did:peer:1` for other agents (AFJ, AFGo)
- In DID Exchange Responses, we use the num algo the requester has used. So if they used `did:peer:2`, we'll respond with a `did:peer:2` as well, regardless of our default setting

Note: when using `did:peer:2`, both DID Exchange Requests and Responses are not adding any signature. There is an [open question](https://github.com/hyperledger/aries-rfcs/issues/717) since the time when DID Exchange was implemented in AFJ: I think we'll need to push to clarify this in order to have a common implementation in both AFJ and ACA-Py.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 15:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1549" class=".btn">#1549</a>
            </td>
            <td>
                <b>
                    fix: create message subscription first
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                mediation initialization was happening before the message subscription was registered, thus meaning the received messages to provision the mediator wouldn't be processed. This moves it to the start of the initialize method, before mediation initialization
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 12:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1548" class=".btn">#1548</a>
            </td>
            <td>
                <b>
                    chore(release): v0.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release version 0.4.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 11:30:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1547" class=".btn">#1547</a>
            </td>
            <td>
                <b>
                    fix(cheqd): make cosmos payer seed optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Makes the cosmos payer seed optional, as you can also used it as a holder without payer seed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 10:45:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1546" class=".btn">#1546</a>
            </td>
            <td>
                <b>
                    feat: Basic Messages V2 for DIDComm V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Refactor Basic Messages modules to support both V1 and V2 protocols. At the moment, in order to not introduce breaking changes in API level, when messages are sent

TODO
- Fix and create new tests
- Add protocolVersion record for BasicMessageRecord. This can be optional and make permanent when making a new release (migration script included)
- Analyze how to support DIDComm V1 for Basic Messages 2.0, as the protocol might work with both versions. This will apply also for Discover Features 2.0 and others

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 12:39:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1545" class=".btn">#1545</a>
            </td>
            <td>
                <b>
                    build(deps): bump protobufjs from 6.11.3 to 6.11.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [protobufjs](https://github.com/protobufjs/protobuf.js) from 6.11.3 to 6.11.4.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/protobufjs/protobuf.js/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=protobufjs&package-manager=npm_and_yarn&previous-version=6.11.3&new-version=6.11.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 22:53:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1544" class=".btn">#1544</a>
            </td>
            <td>
                <b>
                    fix: add OOB id to auto-created connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When a connection is auto-created after receiving first DIDComm v2 message, the OOB record that generated the invitation is not associated to it. So it becomes difficult to find it it afterwards. 

This happened to Faber in the demo, and may happen to you as well!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 23:10:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1543" class=".btn">#1543</a>
            </td>
            <td>
                <b>
                    test: DidCommV2 compatibility with Aries GO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added test and note regarding the compatibility of DidCommV2 message packing with AFGo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 06:16:10 +0000 UTC
    </div>
</div>

