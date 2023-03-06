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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2155" class=".btn">#2155</a>
            </td>
            <td>
                <b>
                    fix: askar exception message always displaying null DID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixing a minor inconvenience where `AskarWallet` error message always displays `Unknown DID: null` when DID is not found in wallet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-06 10:59:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2151" class=".btn">#2151</a>
            </td>
            <td>
                <b>
                    Fix: Performance Demo [no --revocation]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes issue with performance demo [no revocation], where number of issued credentials stops incrementing when received credentials reaches 100% and the demo would eventually timeout.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 16:35:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2150" class=".btn">#2150</a>
            </td>
            <td>
                <b>
                    Problem report generation for Out of band protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creating this PR to add an endpoint to generate problem-report for out of band protocol on the basis of ConnectionId. Looking for the feedback from the community.
-Signed off by: ramreddychalla94 [ram.challa@ontario.ca](mailto:ram.challa@ontario.ca)
-Funded by the Ontario Government

This PR resolves https://github.com/hyperledger/aries-cloudagent-python/issues/2101 @swcurran please review and let us know of your comments, thanks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 06:40:20 +0000 UTC
    </div>
</div>

