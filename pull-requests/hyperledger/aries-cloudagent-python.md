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
- Support both `issue-credential-v1` and `issue-credential-v2` credential offer
- Test coverage
- Current status: final testing
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1304" class=".btn">#1304</a>
            </td>
            <td>
                <b>
                    Update version to 0.7.0-rc1
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
        Created At 2021-07-08 19:52:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1303" class=".btn">#1303</a>
            </td>
            <td>
                <b>
                    DIF PE Integration Test Update - required before PR#1294 merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - This PR is connected to #1294. Keeping this separate for the review process. Once this merged and PR#1294 is updated, I expect all checks to pass.
- Following discussion with @andrewwhitehead, now using `is_holder` to decide whether `VP` should be signed or not. The `VP` cannot be verified unless `is_holder` property is specified in the `presentation_definition` which is causing the tests to fail.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 10:18:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1302" class=".btn">#1302</a>
            </td>
            <td>
                <b>
                    Fix warnings due to action API updates
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
        Created At 2021-07-07 18:53:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1301" class=".btn">#1301</a>
            </td>
            <td>
                <b>
                    fix: failure to verify jsonld on non-conformant doc but vaild vmethod
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor fix for jsonld verify route.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 18:22:59 +0000 UTC
    </div>
</div>

