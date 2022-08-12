---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    update weaver dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 14:35:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/366" class=".btn">#366</a>
            </td>
            <td>
                <b>
                    Upgrade to ginkgo v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">testing</span>
            </td>
            <td>
                This PR upgrades to ginkgo v2 and enables new functionality such as flaky test retry.

In order to overcome an upgrade conflict where we had v1 and v2 in use, this PR also replaces our impl of ordered and parallel runners with the implementations provided by ifrit. While this replacement does solves the conflict, it also reduces our code base.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 14:14:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/364" class=".btn">#364</a>
            </td>
            <td>
                <b>
                    Make ATSA Chaincode receipt struct fields public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue https://github.com/hyperledger-labs/fabric-smart-client/issues/50, removed warnings related to:

SA9005: missing marshaling mechanism

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 12:53:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (U1000)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* U1000: unused variables and functions

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 14:52:49 +0000 UTC
    </div>
</div>

