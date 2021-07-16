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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1318" class=".btn">#1318</a>
            </td>
            <td>
                <b>
                    Typo in acme example + added sentence forclarity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixing typo (line was accidentally commented out), and explaining where to copy paste a code snippet (unclear from the instructions)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 23:54:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1317" class=".btn">#1317</a>
            </td>
            <td>
                <b>
                    Update version to 0.7.0, update to Askar 0.2 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 23:26:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1316" class=".btn">#1316</a>
            </td>
            <td>
                <b>
                    OOB Protocol - CredentialOffer Attachment Support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Extends work done by @DaevMithran in #1216 
- Adds a `create-offer` endpoint in `issue-credential-v1` and `issue-credential-v2` to create an offer independent of connection.
- Support both `issue-credential-v1` and `issue-credential-v2` credential offer workflow 
[Faber] with auto flags, offer_sent -> request_received -> credential_issued
[Alice] with auto flags, offer_received -> request_sent -> credential_received
- Test coverage
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 15:54:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1314" class=".btn">#1314</a>
            </td>
            <td>
                <b>
                    Set DID posture to posted when assigned as the public DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1307

Also avoids a potential failure when two agent processes try to perform the public DID upgrade process simultaneously.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-13 23:17:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1306" class=".btn">#1306</a>
            </td>
            <td>
                <b>
                    Tweaks to AcmeWorkshop Docs -- instruction to use external ledger
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
        Created At 2021-07-09 10:08:52 +0000 UTC
    </div>
</div>

