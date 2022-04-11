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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/702" class=".btn">#702</a>
            </td>
            <td>
                <b>
                    feat: Ability to add Non-secret records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Summary of Changes

Added a non-secret module with minimal API just to expose the on-secret APIs for Indy library [here](https://hyperledger-indy.readthedocs.io/projects/sdk/en/latest/docs/design/003-wallet-storage/README.html#) 
This will enable business logic that requires saving custom records like wallet history to be saved to the wallet and retrieved back when possible

Related Issue #685 




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-09 10:01:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/700" class=".btn">#700</a>
            </td>
            <td>
                <b>
                    feat: use did keys for oob and did exchange protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jakub Koci <jakub.koci@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 15:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/699" class=".btn">#699</a>
            </td>
            <td>
                <b>
                    feat: add support for postgres wallet type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sai Ranjit Tummalapalli <sairanjit.tummalapalli@ayanworks.com>

Related issue: #553 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 13:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/698" class=".btn">#698</a>
            </td>
            <td>
                <b>
                    feat: find existing connection based on invitation did
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I added a function `serviceToNumAlgo2Did` but I'm testing it in `DidPeer.test`, because I was curious if it's possible to create regular PeerDid and then take `didDocument` from it. As you can see it's not possible right now so I commented the code in the test. 

I described what might be a cause of the problem in issue here [RFC 0434: Ambiguous description of Peer DID numalgo 2 service encoding](https://github.com/hyperledger/aries-rfcs/issues/728).

There is also a simplification of when and what invitation did we store in the connection record. OOB invitation can contain more dids (or service blocks encoded as peer did numalgo2) and we should store only the one we successfully use to send connection request message to.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 08:50:39 +0000 UTC
    </div>
</div>

