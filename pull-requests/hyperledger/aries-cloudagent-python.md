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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2149" class=".btn">#2149</a>
            </td>
            <td>
                <b>
                    [fix] Removes extra comma that prevents swagger from accepting the presentation request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue #2146

Signed-off-by: Stephen Curran <swcurran@gmail.com>

Signed-off-by: Stephen Curran <swcurran@cloudcompass.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 17:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2148" class=".btn">#2148</a>
            </td>
            <td>
                <b>
                    Feat: Multiple Presentations [v2.1] 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1756 
- closed original PR#2114 due to issue with rebasing, copied over change here.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 13:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2147" class=".btn">#2147</a>
            </td>
            <td>
                <b>
                    Fix: messages stuck in mediator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #2111

Performance Demo Analysis [No dropoff]
| branch | test config    | time taken |
|---------|--------------------------------------|-----------|
| This PR | 10000 credentials with revocation    | 1107.09 s, 1078.85 s |
| Main    | 10000 credentials with revocation    | 1089.77 s, 1075.61 s |
| This PR | 10000 credentials without revocation | 1035.22 s |
| Main    | 10000 credentials without revocation | 1042.04 s |
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 12:35:13 +0000 UTC
    </div>
</div>

