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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1300" class=".btn">#1300</a>
            </td>
            <td>
                <b>
                    Accept short DIDs for their_public_did parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow-up to https://github.com/hyperledger/aries-cloudagent-python/pull/1296
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 16:27:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1298" class=".btn">#1298</a>
            </td>
            <td>
                <b>
                    check if did is already qualified
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #1296 introduced a problem that  when the `pthid` got set to the public DID in a DIDX request with an already qualified DID it would still get prefixed with `did:sov`.


Signed-off-by: Woerner Dominic (RBCH/PJ-IOT) <dominic.woerner2@ch.bosch.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 17:35:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1297" class=".btn">#1297</a>
            </td>
            <td>
                <b>
                    Update version to 0.7.0-rc0
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
        Created At 2021-07-06 15:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1296" class=".btn">#1296</a>
            </td>
            <td>
                <b>
                    Support generic public DIDs in DIDX request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Be more permissive in validation of target public DID in `didexchange/create-request`.
Public DIDs are resolved using the resolver interface which supports additional DID methods besides `did:sov` (e.g. `did:web`).

Only question is if we should still allow unqualified DIDs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 12:56:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1294" class=".btn">#1294</a>
            </td>
            <td>
                <b>
                    DIF PE - is_holder property implementation - compliant with DIF spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1261
- I think this meets the following attributes from the DIF spec ~~but does not use the `is_holder` property to decide whether the `VP` should be signed or not. But in case, this is needed then this can be done with minimal changes/extension~~.
1. `Verify that the Holder or Subject of the Claim still controls the identifier [DID].` [Link](https://identity.foundation/presentation-exchange/#proof-of-identifier-control)
2. `Holder of  Claim is the same as the Subject of the attribute.` [Link](https://identity.foundation/presentation-exchange/#note-2) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 11:21:00 +0000 UTC
    </div>
</div>

