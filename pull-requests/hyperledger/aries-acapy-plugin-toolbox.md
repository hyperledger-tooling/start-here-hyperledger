---
layout: default
title: aries-acapy-plugin-toolbox
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugin-toolbox
---

# aries-acapy-plugin-toolbox <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugin-toolbox){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    feat/added_deletehandler_unit_test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: PeterStrob <peter@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 20:21:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    feat:added_StorageError_check_to_updatehandler_test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a check for the StorageError exception to the UpdateHandler test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 16:28:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    fix: Switch from Sovrin StagingNet to BuilderNet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Due to a recent change, the StagingNet is no longer free. It is
recommended that developers switch to the BuilderNet for development
purposes. If an application reaches a state where it is applicable for a
prototype or pre-production uses, the StagingNet should be used instead.

Please see https://selfserve.sovrin.org/ for more information about the
different Sovrin networks.

This commit changes all references to the StagingNet to point to the
BuilderNet instead.

Signed-off-by: Colton Wolkins (Indicio work address) <colton@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 17:26:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    feat:added updatehandler test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added unit test for UpdateHandler class, as well as fixed bug in class. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 22:33:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    fix: demo mediator use undelivered queue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 19:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugin-toolbox/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    Add presentation request to the "get-matching-credentials" call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When requesting matching credentials to a presentation, the credentials are returned without any indication of what the verifier requested. This change adds the presentation request to the response which will reduce API requests and unneeded complexity for the prover.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 11:13:12 +0000 UTC
    </div>
</div>

