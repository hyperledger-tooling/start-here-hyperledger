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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    feat: Pack and send message based on DidDoc services
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to #268 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 10:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    docs: complete documentation overhaul
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This would allow for an easier introduction to this framework. We felt that the previous docs contained too much unstructured information and this should fix that.

The docs folder is also setup for gitbooks, which will allow for an even better "getting-started-experience"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 10:13:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    Mediation: fix autoAcceptMediationRequests flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a missing behaviour from last merge regarding mediation request handling (do not automatically grant mediation if autoAcceptMediationRequests flag is set).

There is some progress on e2e tests using mediation modules, attempting to support different transports (today only http).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 06:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    Debug mediation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                passing test in e2e tests that establishes a mediation relationship. This includes needed code for mediation server-side as well as client-side. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 17:03:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    fix: use both thread id and connection id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Using only the thread id gives errors when issuing or proving to yourself as there are multiple records for a single thread id. This retrieves records by both thread id an connection id. this also removes the requirement to check if the record has the correct connection id.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 13:43:31 +0000 UTC
    </div>
</div>

